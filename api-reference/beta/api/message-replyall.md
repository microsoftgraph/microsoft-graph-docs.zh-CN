---
title: 消息：replyAll
description: '通过指定注释和修改任何可更新属性回复邮件的所有收件人 '
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 05f552676400196aed275c32020bcdf5211d0e31
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528611"
---
# <a name="message-replyall"></a><span data-ttu-id="667fb-103">消息：replyAll</span><span class="sxs-lookup"><span data-stu-id="667fb-103">message: replyAll</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="667fb-104">通过指定注释和所有使用**replyAll**方法修改的回复，任何可更新属性回复邮件的所有收件人。</span><span class="sxs-lookup"><span data-stu-id="667fb-104">Reply to all recipients of a message by specifying a comment and modifying any updateable properties for the reply, all by using the **replyAll** method.</span></span> <span data-ttu-id="667fb-105">然后在已发送邮件文件夹中保存邮件。</span><span class="sxs-lookup"><span data-stu-id="667fb-105">The message is then saved in the Sent Items folder.</span></span>

<span data-ttu-id="667fb-106">此外，您可以第一个[创建草稿全部答复邮件](../api/message-createreplyall.md)包含评论或更新任何消息属性，然后[发送](../api/message-send.md)答复。</span><span class="sxs-lookup"><span data-stu-id="667fb-106">Alternatively, you can first [create a draft reply-all message](../api/message-createreplyall.md) to include a comment or update any message properties, and then [send](../api/message-send.md) the reply.</span></span>

<span data-ttu-id="667fb-107">**注意**</span><span class="sxs-lookup"><span data-stu-id="667fb-107">**Note**</span></span>

- <span data-ttu-id="667fb-108">您可以指定注释或的**body**属性`message`参数。</span><span class="sxs-lookup"><span data-stu-id="667fb-108">You can specify either a comment or the **body** property of the `message` parameter.</span></span> <span data-ttu-id="667fb-109">如果同时指定将返回 HTTP 400 错误请求出错。</span><span class="sxs-lookup"><span data-stu-id="667fb-109">Specifying both will return an HTTP 400 Bad Request error.</span></span>
- <span data-ttu-id="667fb-110">如果**回复**属性指定在原始邮件中，每个 Internet 邮件格式 ([RFC 2822](https://www.rfc-editor.org/info/rfc2822))，您应发送给收件人的答复</span><span class="sxs-lookup"><span data-stu-id="667fb-110">If the **replyTo** property is specified in the original message, per Internet Message Format ([RFC 2822](https://www.rfc-editor.org/info/rfc2822)), you should send the reply to the recipients in the</span></span>  
<span data-ttu-id="667fb-111">**回复**和**toRecipients**属性，并不**从**和**toRecipients**属性中的收件人。</span><span class="sxs-lookup"><span data-stu-id="667fb-111">**replyTo** and **toRecipients** properties, and not the recipients in the **from** and **toRecipients** properties.</span></span> 


## <a name="permissions"></a><span data-ttu-id="667fb-112">权限</span><span class="sxs-lookup"><span data-stu-id="667fb-112">Permissions</span></span>
<span data-ttu-id="667fb-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="667fb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="667fb-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="667fb-115">Permission type</span></span>      | <span data-ttu-id="667fb-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="667fb-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="667fb-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="667fb-117">Delegated (work or school account)</span></span> | <span data-ttu-id="667fb-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="667fb-118">Mail.Send</span></span>    |
|<span data-ttu-id="667fb-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="667fb-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="667fb-120">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="667fb-120">Mail.Send</span></span>    |
|<span data-ttu-id="667fb-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="667fb-121">Application</span></span> | <span data-ttu-id="667fb-122">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="667fb-122">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="667fb-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="667fb-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/me/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/messages/{id}/replyAll
POST /me/mailFolders/{id}/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/replyAll
```
## <a name="request-headers"></a><span data-ttu-id="667fb-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="667fb-124">Request headers</span></span>
| <span data-ttu-id="667fb-125">名称</span><span class="sxs-lookup"><span data-stu-id="667fb-125">Name</span></span>       | <span data-ttu-id="667fb-126">类型</span><span class="sxs-lookup"><span data-stu-id="667fb-126">Type</span></span> | <span data-ttu-id="667fb-127">说明</span><span class="sxs-lookup"><span data-stu-id="667fb-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="667fb-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="667fb-128">Authorization</span></span>  | <span data-ttu-id="667fb-129">string</span><span class="sxs-lookup"><span data-stu-id="667fb-129">string</span></span>  | <span data-ttu-id="667fb-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="667fb-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="667fb-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="667fb-132">Content-Type</span></span> | <span data-ttu-id="667fb-133">string</span><span class="sxs-lookup"><span data-stu-id="667fb-133">string</span></span>  | <span data-ttu-id="667fb-p105">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="667fb-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="667fb-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="667fb-136">Request body</span></span>
<span data-ttu-id="667fb-137">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="667fb-137">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="667fb-138">参数</span><span class="sxs-lookup"><span data-stu-id="667fb-138">Parameter</span></span>    | <span data-ttu-id="667fb-139">类型</span><span class="sxs-lookup"><span data-stu-id="667fb-139">Type</span></span>   |<span data-ttu-id="667fb-140">说明</span><span class="sxs-lookup"><span data-stu-id="667fb-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="667fb-141">注释</span><span class="sxs-lookup"><span data-stu-id="667fb-141">comment</span></span>|<span data-ttu-id="667fb-142">String</span><span class="sxs-lookup"><span data-stu-id="667fb-142">String</span></span>|<span data-ttu-id="667fb-p106">要包含的注释。可以为空字符串。</span><span class="sxs-lookup"><span data-stu-id="667fb-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="667fb-145">message</span><span class="sxs-lookup"><span data-stu-id="667fb-145">message</span></span>|[<span data-ttu-id="667fb-146">message</span><span class="sxs-lookup"><span data-stu-id="667fb-146">message</span></span>](../resources/message.md)|<span data-ttu-id="667fb-147">若要在答复邮件更新任何可写属性。</span><span class="sxs-lookup"><span data-stu-id="667fb-147">Any writeable properties to update in the reply message.</span></span>|

## <a name="response"></a><span data-ttu-id="667fb-148">响应</span><span class="sxs-lookup"><span data-stu-id="667fb-148">Response</span></span>

<span data-ttu-id="667fb-p107">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="667fb-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="667fb-151">示例</span><span class="sxs-lookup"><span data-stu-id="667fb-151">Example</span></span>
<span data-ttu-id="667fb-152">下面的示例包括一条注释，并将添加到全部答复邮件附件。</span><span class="sxs-lookup"><span data-stu-id="667fb-152">The following example includes a comment and adds an attachment to the reply-all message.</span></span>
##### <a name="request"></a><span data-ttu-id="667fb-153">请求</span><span class="sxs-lookup"><span data-stu-id="667fb-153">Request</span></span>
<span data-ttu-id="667fb-154">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="667fb-154">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_replyall"
}-->
```http
POST https://graph.microsoft.com/beta/me/messages/AAMkADA1MTAAAH5JaKAAA=/replyAll
Content-Type: application/json

{
    "message":{
      "attachments": [ 
        { 
          "@odata.type": "#microsoft.graph.fileAttachment", 
          "name": "guidelines.txt", 
          "contentBytes": "bWFjIGFuZCBjaGVlc2UgdG9kYXk=" 
        } 
      ]
    },
    "comment": "Please take a look at the attached guidelines before you decide on the name." 
}
```


##### <a name="response"></a><span data-ttu-id="667fb-155">响应</span><span class="sxs-lookup"><span data-stu-id="667fb-155">Response</span></span>
<span data-ttu-id="667fb-156">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="667fb-156">Here is an example of the response.</span></span>
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
  "description": "message: replyAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/message-replyall.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
