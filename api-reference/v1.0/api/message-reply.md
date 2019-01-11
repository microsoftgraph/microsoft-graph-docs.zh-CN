---
title: 消息：答复
description: 答复邮件发件人然后邮件保存在已发送邮件文件夹中。
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 2ba3df6551aab9138e90fa5e3fc452f2929b4815
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27856320"
---
# <a name="message-reply"></a><span data-ttu-id="55385-104">消息：答复</span><span class="sxs-lookup"><span data-stu-id="55385-104">message: reply</span></span>

<span data-ttu-id="55385-p102">答复邮件发件人然后邮件保存在已发送邮件文件夹中。</span><span class="sxs-lookup"><span data-stu-id="55385-p102">Reply to the sender of a message. The message is then saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="55385-107">权限</span><span class="sxs-lookup"><span data-stu-id="55385-107">Permissions</span></span>
<span data-ttu-id="55385-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="55385-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55385-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="55385-110">Permission type</span></span>      | <span data-ttu-id="55385-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="55385-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="55385-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="55385-112">Delegated (work or school account)</span></span> | <span data-ttu-id="55385-113">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="55385-113">Mail.Send</span></span>    |
|<span data-ttu-id="55385-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="55385-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="55385-115">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="55385-115">Mail.Send</span></span>    |
|<span data-ttu-id="55385-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="55385-116">Application</span></span> | <span data-ttu-id="55385-117">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="55385-117">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="55385-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="55385-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/messages/{id}/reply
POST /users/{id | userPrincipalName}/messages/{id}/reply
POST /me/mailFolders/{id}/messages/{id}/reply
POST /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/reply
```
## <a name="request-headers"></a><span data-ttu-id="55385-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="55385-119">Request headers</span></span>
| <span data-ttu-id="55385-120">名称</span><span class="sxs-lookup"><span data-stu-id="55385-120">Name</span></span>       | <span data-ttu-id="55385-121">类型</span><span class="sxs-lookup"><span data-stu-id="55385-121">Type</span></span> | <span data-ttu-id="55385-122">说明</span><span class="sxs-lookup"><span data-stu-id="55385-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="55385-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="55385-123">Authorization</span></span>  | <span data-ttu-id="55385-124">string</span><span class="sxs-lookup"><span data-stu-id="55385-124">string</span></span>  | <span data-ttu-id="55385-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="55385-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="55385-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="55385-127">Content-Type</span></span> | <span data-ttu-id="55385-128">string</span><span class="sxs-lookup"><span data-stu-id="55385-128">string</span></span>  | <span data-ttu-id="55385-p105">实体正文中的数据性质。必需。</span><span class="sxs-lookup"><span data-stu-id="55385-p105">Nature of the data in the body of an entity. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="55385-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="55385-131">Request body</span></span>
<span data-ttu-id="55385-132">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="55385-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="55385-133">参数</span><span class="sxs-lookup"><span data-stu-id="55385-133">Parameter</span></span>    | <span data-ttu-id="55385-134">类型</span><span class="sxs-lookup"><span data-stu-id="55385-134">Type</span></span>   |<span data-ttu-id="55385-135">说明</span><span class="sxs-lookup"><span data-stu-id="55385-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="55385-136">注释</span><span class="sxs-lookup"><span data-stu-id="55385-136">comment</span></span>|<span data-ttu-id="55385-137">String</span><span class="sxs-lookup"><span data-stu-id="55385-137">String</span></span>|<span data-ttu-id="55385-p106">要包含的注释。可以为空字符串。</span><span class="sxs-lookup"><span data-stu-id="55385-p106">A comment to include. Can be an empty string.</span></span>|

## <a name="response"></a><span data-ttu-id="55385-140">响应</span><span class="sxs-lookup"><span data-stu-id="55385-140">Response</span></span>

<span data-ttu-id="55385-p107">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="55385-p107">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55385-143">示例</span><span class="sxs-lookup"><span data-stu-id="55385-143">Example</span></span>
<span data-ttu-id="55385-144">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="55385-144">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="55385-145">请求</span><span class="sxs-lookup"><span data-stu-id="55385-145">Request</span></span>
<span data-ttu-id="55385-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="55385-146">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_reply"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/reply
Content-type: application/json
Content-length: 32

{
  "comment": "comment-value"
}
```

##### <a name="response"></a><span data-ttu-id="55385-147">响应</span><span class="sxs-lookup"><span data-stu-id="55385-147">Response</span></span>
##### <a name="response"></a><span data-ttu-id="55385-148">响应</span><span class="sxs-lookup"><span data-stu-id="55385-148">Response</span></span>
<span data-ttu-id="55385-149">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="55385-149">Here is an example of the response.</span></span>
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
  "description": "message: reply",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
