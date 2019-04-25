---
title: 邮件：转发
description: '转发邮件、添加注释或修改任何可更新的属性  '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: ed3d51c28e6fe0404b5cb26fb17f6d8ed3bba212
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32540473"
---
# <a name="message-forward"></a><span data-ttu-id="2fa59-103">邮件：转发</span><span class="sxs-lookup"><span data-stu-id="2fa59-103">message: forward</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2fa59-104">转发邮件、添加注释或修改任何可更新的属性</span><span class="sxs-lookup"><span data-stu-id="2fa59-104">Forward a message, add a comment or modify any updateable properties</span></span>  
<span data-ttu-id="2fa59-105">一个**正向**调用中的全部。</span><span class="sxs-lookup"><span data-stu-id="2fa59-105">all in one **forward** call.</span></span> <span data-ttu-id="2fa59-106">邮件保存在已发送邮件文件夹中。</span><span class="sxs-lookup"><span data-stu-id="2fa59-106">The message is saved in the Sent Items folder.</span></span>

<span data-ttu-id="2fa59-107">或者, 您可以先[创建一个草稿转发邮件](../api/message-createforward.md), 以包含注释或更新任何邮件属性, 然后[发送](../api/message-send.md)草稿邮件。</span><span class="sxs-lookup"><span data-stu-id="2fa59-107">Alternatively, you can first [create a draft forward message](../api/message-createforward.md) to include a comment or update any message properties, and then [send](../api/message-send.md) the draft message.</span></span>

<span data-ttu-id="2fa59-108">**注意**</span><span class="sxs-lookup"><span data-stu-id="2fa59-108">**Note**</span></span>

- <span data-ttu-id="2fa59-109">您可以指定`message`参数的注释或**body**属性。</span><span class="sxs-lookup"><span data-stu-id="2fa59-109">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="2fa59-110">同时指定这两个将返回 HTTP 400 错误的请求错误。</span><span class="sxs-lookup"><span data-stu-id="2fa59-110">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="2fa59-111">您必须指定`toRecipients`参数或`message`参数的**toRecipients**属性。</span><span class="sxs-lookup"><span data-stu-id="2fa59-111">You must specify either the `toRecipients` parameter or the **toRecipients** property of the `message` parameter.</span></span> <span data-ttu-id="2fa59-112">同时指定或指定两者均不会返回 HTTP 400 错误请求错误。</span><span class="sxs-lookup"><span data-stu-id="2fa59-112">Specifying both or specifying neither will return an HTTP 400 Bad Request error.</span></span>

## <a name="permissions"></a><span data-ttu-id="2fa59-113">权限</span><span class="sxs-lookup"><span data-stu-id="2fa59-113">Permissions</span></span>
<span data-ttu-id="2fa59-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2fa59-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2fa59-116">权限类型</span><span class="sxs-lookup"><span data-stu-id="2fa59-116">Permission type</span></span>      | <span data-ttu-id="2fa59-117">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2fa59-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2fa59-118">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2fa59-118">Delegated (work or school account)</span></span> | <span data-ttu-id="2fa59-119">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="2fa59-119">Mail.Send</span></span>    |
|<span data-ttu-id="2fa59-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2fa59-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2fa59-121">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="2fa59-121">Mail.Send</span></span>    |
|<span data-ttu-id="2fa59-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="2fa59-122">Application</span></span> | <span data-ttu-id="2fa59-123">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="2fa59-123">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="2fa59-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2fa59-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/forward
POST /users/{id | userPrincipalName}/messages/{id}/forward
POST /me/mailFolders/{id}/messages/{id}/forward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/forward
```
## <a name="request-headers"></a><span data-ttu-id="2fa59-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="2fa59-125">Request headers</span></span>
| <span data-ttu-id="2fa59-126">名称</span><span class="sxs-lookup"><span data-stu-id="2fa59-126">Name</span></span>       | <span data-ttu-id="2fa59-127">类型</span><span class="sxs-lookup"><span data-stu-id="2fa59-127">Type</span></span> | <span data-ttu-id="2fa59-128">说明</span><span class="sxs-lookup"><span data-stu-id="2fa59-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2fa59-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="2fa59-129">Authorization</span></span>  | <span data-ttu-id="2fa59-130">string</span><span class="sxs-lookup"><span data-stu-id="2fa59-130">string</span></span>  | <span data-ttu-id="2fa59-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2fa59-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2fa59-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2fa59-133">Content-Type</span></span> | <span data-ttu-id="2fa59-134">string</span><span class="sxs-lookup"><span data-stu-id="2fa59-134">string</span></span>  | <span data-ttu-id="2fa59-p106">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="2fa59-p106">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2fa59-137">请求正文</span><span class="sxs-lookup"><span data-stu-id="2fa59-137">Request body</span></span>
<span data-ttu-id="2fa59-138">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="2fa59-138">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2fa59-139">参数</span><span class="sxs-lookup"><span data-stu-id="2fa59-139">Parameter</span></span>    | <span data-ttu-id="2fa59-140">类型</span><span class="sxs-lookup"><span data-stu-id="2fa59-140">Type</span></span>   |<span data-ttu-id="2fa59-141">说明</span><span class="sxs-lookup"><span data-stu-id="2fa59-141">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2fa59-142">注释</span><span class="sxs-lookup"><span data-stu-id="2fa59-142">comment</span></span>|<span data-ttu-id="2fa59-143">String</span><span class="sxs-lookup"><span data-stu-id="2fa59-143">String</span></span>|<span data-ttu-id="2fa59-p107">要包含的注释。可以为空字符串。</span><span class="sxs-lookup"><span data-stu-id="2fa59-p107">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="2fa59-146">toRecipients</span><span class="sxs-lookup"><span data-stu-id="2fa59-146">toRecipients</span></span>|<span data-ttu-id="2fa59-147">[recipient](../resources/recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="2fa59-147">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="2fa59-148">收件人列表</span><span class="sxs-lookup"><span data-stu-id="2fa59-148">The list of recipients.</span></span>|
|<span data-ttu-id="2fa59-149">message</span><span class="sxs-lookup"><span data-stu-id="2fa59-149">message</span></span>|[<span data-ttu-id="2fa59-150">邮件</span><span class="sxs-lookup"><span data-stu-id="2fa59-150">message</span></span>](../resources/message.md)|<span data-ttu-id="2fa59-151">答复邮件中要更新的任何可写属性。</span><span class="sxs-lookup"><span data-stu-id="2fa59-151">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="2fa59-152">响应</span><span class="sxs-lookup"><span data-stu-id="2fa59-152">Response</span></span>

<span data-ttu-id="2fa59-p108">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="2fa59-p108">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2fa59-155">示例</span><span class="sxs-lookup"><span data-stu-id="2fa59-155">Example</span></span>
<span data-ttu-id="2fa59-156">下面的示例将**isDeliveryReceiptRequested**属性设置为 true, 添加注释并转发邮件。</span><span class="sxs-lookup"><span data-stu-id="2fa59-156">The following example sets the **isDeliveryReceiptRequested** property to true, adds a comment and forwards the message.</span></span>
##### <a name="request"></a><span data-ttu-id="2fa59-157">请求</span><span class="sxs-lookup"><span data-stu-id="2fa59-157">Request</span></span>
<span data-ttu-id="2fa59-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2fa59-158">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="2fa59-159">响应</span><span class="sxs-lookup"><span data-stu-id="2fa59-159">Response</span></span>
<span data-ttu-id="2fa59-160">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="2fa59-160">Here is an example of the response.</span></span>
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
