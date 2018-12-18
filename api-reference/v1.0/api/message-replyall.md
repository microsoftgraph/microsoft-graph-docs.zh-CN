---
title: 消息：replyAll
description: 答复邮件的所有收件人。然后邮件保存在已发送邮件文件夹中。
author: angelgolfer-ms
ms.openlocfilehash: cefe4d92d23cb9531f6fa66f74d1c9af87ef429e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27348984"
---
# <a name="message-replyall"></a><span data-ttu-id="1c2a6-104">消息：replyAll</span><span class="sxs-lookup"><span data-stu-id="1c2a6-104">message: replyAll</span></span>

<span data-ttu-id="1c2a6-p102">答复邮件的所有收件人。然后邮件保存在已发送邮件文件夹中。</span><span class="sxs-lookup"><span data-stu-id="1c2a6-p102">Reply to all recipients of a message. The message is then saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="1c2a6-107">权限</span><span class="sxs-lookup"><span data-stu-id="1c2a6-107">Permissions</span></span>
<span data-ttu-id="1c2a6-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1c2a6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c2a6-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1c2a6-110">Permission type</span></span>      | <span data-ttu-id="1c2a6-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1c2a6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1c2a6-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1c2a6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1c2a6-113">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="1c2a6-113">Mail.Send</span></span>    |
|<span data-ttu-id="1c2a6-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1c2a6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c2a6-115">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="1c2a6-115">Mail.Send</span></span>    |
|<span data-ttu-id="1c2a6-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="1c2a6-116">Application</span></span> | <span data-ttu-id="1c2a6-117">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="1c2a6-117">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="1c2a6-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1c2a6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/me/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/messages/{id}/replyAll
POST /me/mailFolders/{id}/messages/{id}/replyAll
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/replyAll
```
## <a name="request-headers"></a><span data-ttu-id="1c2a6-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="1c2a6-119">Request headers</span></span>
| <span data-ttu-id="1c2a6-120">Name</span><span class="sxs-lookup"><span data-stu-id="1c2a6-120">Name</span></span>       | <span data-ttu-id="1c2a6-121">类型</span><span class="sxs-lookup"><span data-stu-id="1c2a6-121">Type</span></span> | <span data-ttu-id="1c2a6-122">说明</span><span class="sxs-lookup"><span data-stu-id="1c2a6-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1c2a6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1c2a6-123">Authorization</span></span>  | <span data-ttu-id="1c2a6-124">string</span><span class="sxs-lookup"><span data-stu-id="1c2a6-124">string</span></span>  | <span data-ttu-id="1c2a6-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1c2a6-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1c2a6-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1c2a6-127">Content-Type</span></span> | <span data-ttu-id="1c2a6-128">string</span><span class="sxs-lookup"><span data-stu-id="1c2a6-128">string</span></span>  | <span data-ttu-id="1c2a6-p105">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="1c2a6-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1c2a6-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="1c2a6-131">Request body</span></span>
<span data-ttu-id="1c2a6-132">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="1c2a6-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="1c2a6-133">参数</span><span class="sxs-lookup"><span data-stu-id="1c2a6-133">Parameter</span></span>    | <span data-ttu-id="1c2a6-134">Type</span><span class="sxs-lookup"><span data-stu-id="1c2a6-134">Type</span></span>   |<span data-ttu-id="1c2a6-135">说明</span><span class="sxs-lookup"><span data-stu-id="1c2a6-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1c2a6-136">注释</span><span class="sxs-lookup"><span data-stu-id="1c2a6-136">comment</span></span>|<span data-ttu-id="1c2a6-137">String</span><span class="sxs-lookup"><span data-stu-id="1c2a6-137">String</span></span>|<span data-ttu-id="1c2a6-p106">要包含的注释。可以为空字符串。</span><span class="sxs-lookup"><span data-stu-id="1c2a6-p106">A comment to include. Can be an empty string.</span></span>|

## <a name="response"></a><span data-ttu-id="1c2a6-140">响应</span><span class="sxs-lookup"><span data-stu-id="1c2a6-140">Response</span></span>

<span data-ttu-id="1c2a6-p107">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="1c2a6-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c2a6-143">示例</span><span class="sxs-lookup"><span data-stu-id="1c2a6-143">Example</span></span>
<span data-ttu-id="1c2a6-144">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="1c2a6-144">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1c2a6-145">请求</span><span class="sxs-lookup"><span data-stu-id="1c2a6-145">Request</span></span>
<span data-ttu-id="1c2a6-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1c2a6-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_replyall"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/replyAll
Content-type: application/json
Content-length: 32

{
  "comment": "comment-value"
}
```


##### <a name="response"></a><span data-ttu-id="1c2a6-147">响应</span><span class="sxs-lookup"><span data-stu-id="1c2a6-147">Response</span></span>
<span data-ttu-id="1c2a6-148">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="1c2a6-148">Here is an example of the response.</span></span>
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
  "description": "message: replyAll",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
