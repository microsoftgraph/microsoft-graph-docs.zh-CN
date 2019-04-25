---
title: 邮件：转发
description: 转发邮件。邮件保存在已发送邮件文件夹中。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 12409685e21b338a86b392f32449b006a0e958f7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581742"
---
# <a name="message-forward"></a><span data-ttu-id="3ffff-104">邮件：转发</span><span class="sxs-lookup"><span data-stu-id="3ffff-104">message: forward</span></span>

<span data-ttu-id="3ffff-p102">转发邮件。邮件保存在已发送邮件文件夹中。</span><span class="sxs-lookup"><span data-stu-id="3ffff-p102">Forward a message. The message is saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="3ffff-107">权限</span><span class="sxs-lookup"><span data-stu-id="3ffff-107">Permissions</span></span>
<span data-ttu-id="3ffff-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3ffff-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ffff-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3ffff-110">Permission type</span></span>      | <span data-ttu-id="3ffff-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3ffff-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3ffff-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3ffff-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3ffff-113">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="3ffff-113">Mail.Send</span></span>    |
|<span data-ttu-id="3ffff-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3ffff-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ffff-115">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="3ffff-115">Mail.Send</span></span>    |
|<span data-ttu-id="3ffff-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="3ffff-116">Application</span></span> | <span data-ttu-id="3ffff-117">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="3ffff-117">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="3ffff-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3ffff-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/forward
POST /users/{id | userPrincipalName}/messages/{id}/forward
POST /me/mailFolders/{id}/messages/{id}/forward
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/forward
```
## <a name="request-headers"></a><span data-ttu-id="3ffff-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="3ffff-119">Request headers</span></span>
| <span data-ttu-id="3ffff-120">名称</span><span class="sxs-lookup"><span data-stu-id="3ffff-120">Name</span></span>       | <span data-ttu-id="3ffff-121">类型</span><span class="sxs-lookup"><span data-stu-id="3ffff-121">Type</span></span> | <span data-ttu-id="3ffff-122">说明</span><span class="sxs-lookup"><span data-stu-id="3ffff-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3ffff-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ffff-123">Authorization</span></span>  | <span data-ttu-id="3ffff-124">string</span><span class="sxs-lookup"><span data-stu-id="3ffff-124">string</span></span>  | <span data-ttu-id="3ffff-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3ffff-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3ffff-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3ffff-127">Content-Type</span></span> | <span data-ttu-id="3ffff-128">string</span><span class="sxs-lookup"><span data-stu-id="3ffff-128">string</span></span>  | <span data-ttu-id="3ffff-p105">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="3ffff-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3ffff-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="3ffff-131">Request body</span></span>
<span data-ttu-id="3ffff-132">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="3ffff-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3ffff-133">参数</span><span class="sxs-lookup"><span data-stu-id="3ffff-133">Parameter</span></span>    | <span data-ttu-id="3ffff-134">类型</span><span class="sxs-lookup"><span data-stu-id="3ffff-134">Type</span></span>   |<span data-ttu-id="3ffff-135">说明</span><span class="sxs-lookup"><span data-stu-id="3ffff-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3ffff-136">注释</span><span class="sxs-lookup"><span data-stu-id="3ffff-136">comment</span></span>|<span data-ttu-id="3ffff-137">String</span><span class="sxs-lookup"><span data-stu-id="3ffff-137">String</span></span>|<span data-ttu-id="3ffff-p106">要包含的注释。可以为空字符串。</span><span class="sxs-lookup"><span data-stu-id="3ffff-p106">A comment to include. Can be an empty string.</span></span>|
|<span data-ttu-id="3ffff-140">toRecipients</span><span class="sxs-lookup"><span data-stu-id="3ffff-140">toRecipients</span></span>|<span data-ttu-id="3ffff-141">[Recipient](../resources/recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="3ffff-141">[Recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="3ffff-142">收件人列表</span><span class="sxs-lookup"><span data-stu-id="3ffff-142">The list of recipients.</span></span>|

## <a name="response"></a><span data-ttu-id="3ffff-143">响应</span><span class="sxs-lookup"><span data-stu-id="3ffff-143">Response</span></span>

<span data-ttu-id="3ffff-p107">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="3ffff-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ffff-146">示例</span><span class="sxs-lookup"><span data-stu-id="3ffff-146">Example</span></span>
<span data-ttu-id="3ffff-147">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="3ffff-147">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="3ffff-148">请求</span><span class="sxs-lookup"><span data-stu-id="3ffff-148">Request</span></span>
<span data-ttu-id="3ffff-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3ffff-149">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_forward"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/forward
Content-type: application/json
Content-length: 166

{
  "comment": "comment-value",
  "toRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ]
}
```

##### <a name="response"></a><span data-ttu-id="3ffff-150">响应</span><span class="sxs-lookup"><span data-stu-id="3ffff-150">Response</span></span>
##### <a name="response"></a><span data-ttu-id="3ffff-151">响应</span><span class="sxs-lookup"><span data-stu-id="3ffff-151">Response</span></span>
<span data-ttu-id="3ffff-152">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="3ffff-152">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
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
