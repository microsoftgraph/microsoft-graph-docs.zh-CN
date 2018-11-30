---
title: 邮件：发送
description: 在草稿文件夹发送邮件。 草稿消息可以是新的邮件草稿、 答复草稿、 全部答复草稿或
ms.openlocfilehash: b295cd5b234bf9dafe1fbba44a03cdc6e9c1842e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047281"
---
# <a name="message-send"></a><span data-ttu-id="824f6-104">邮件：发送</span><span class="sxs-lookup"><span data-stu-id="824f6-104">message: send</span></span>

> <span data-ttu-id="824f6-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="824f6-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="824f6-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="824f6-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="824f6-p103">在草稿箱文件夹中发送邮件。邮件草稿可以是新邮件草稿、答复草稿、全部答复草稿或转发草稿。然后邮件保存在已发送邮件文件夹中。</span><span class="sxs-lookup"><span data-stu-id="824f6-p103">Send a message in the draft folder. The draft message can be a new message draft, reply draft, reply-all draft, or a forward draft. The message is then saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="824f6-110">权限</span><span class="sxs-lookup"><span data-stu-id="824f6-110">Permissions</span></span>

<span data-ttu-id="824f6-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="824f6-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="824f6-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="824f6-113">Permission type</span></span>      | <span data-ttu-id="824f6-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="824f6-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="824f6-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="824f6-115">Delegated (work or school account)</span></span> | <span data-ttu-id="824f6-116">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="824f6-116">Mail.Send</span></span>    |
|<span data-ttu-id="824f6-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="824f6-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="824f6-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="824f6-118">Mail.Send</span></span>    |
|<span data-ttu-id="824f6-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="824f6-119">Application</span></span> | <span data-ttu-id="824f6-120">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="824f6-120">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="824f6-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="824f6-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/send
POST /users/{id | userPrincipalName}/messages/{id}/send
```

## <a name="request-headers"></a><span data-ttu-id="824f6-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="824f6-122">Request headers</span></span>

| <span data-ttu-id="824f6-123">名称</span><span class="sxs-lookup"><span data-stu-id="824f6-123">Name</span></span>       | <span data-ttu-id="824f6-124">类型</span><span class="sxs-lookup"><span data-stu-id="824f6-124">Type</span></span> | <span data-ttu-id="824f6-125">说明</span><span class="sxs-lookup"><span data-stu-id="824f6-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="824f6-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="824f6-126">Authorization</span></span>  | <span data-ttu-id="824f6-127">string</span><span class="sxs-lookup"><span data-stu-id="824f6-127">string</span></span>  | <span data-ttu-id="824f6-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="824f6-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="824f6-130">Content-Length</span><span class="sxs-lookup"><span data-stu-id="824f6-130">Content-Length</span></span> | <span data-ttu-id="824f6-131">number</span><span class="sxs-lookup"><span data-stu-id="824f6-131">number</span></span> | <span data-ttu-id="824f6-132">0。 被必需。</span><span class="sxs-lookup"><span data-stu-id="824f6-132">0. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="824f6-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="824f6-133">Request body</span></span>

## <a name="response"></a><span data-ttu-id="824f6-134">响应</span><span class="sxs-lookup"><span data-stu-id="824f6-134">Response</span></span>

<span data-ttu-id="824f6-p106">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="824f6-p106">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="824f6-137">示例</span><span class="sxs-lookup"><span data-stu-id="824f6-137">Example</span></span>

<span data-ttu-id="824f6-138">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="824f6-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="824f6-139">请求</span><span class="sxs-lookup"><span data-stu-id="824f6-139">Request</span></span>

<span data-ttu-id="824f6-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="824f6-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_send"
}-->

```http
POST https://graph.microsoft.com/beta/me/messages/{id}/send
```

##### <a name="response"></a><span data-ttu-id="824f6-141">响应</span><span class="sxs-lookup"><span data-stu-id="824f6-141">Response</span></span>

<span data-ttu-id="824f6-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="824f6-142">Here is an example of the response.</span></span>
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
  "description": "message: send",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
