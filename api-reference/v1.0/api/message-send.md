---
title: 邮件：发送
description: 在草稿文件夹发送邮件。 草稿消息可以是新的邮件草稿、 答复草稿、 全部答复草稿或
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 3f9740f74238012571abcfa7f406fd12ed58c9e8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977057"
---
# <a name="message-send"></a><span data-ttu-id="9fba0-104">邮件：发送</span><span class="sxs-lookup"><span data-stu-id="9fba0-104">message: send</span></span>

<span data-ttu-id="9fba0-p102">在草稿箱文件夹中发送邮件。邮件草稿可以是新邮件草稿、答复草稿、全部答复草稿或转发草稿。然后邮件保存在已发送邮件文件夹中。</span><span class="sxs-lookup"><span data-stu-id="9fba0-p102">Send a message in the draft folder. The draft message can be a new message draft, reply draft, reply-all draft, or a forward draft. The message is then saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="9fba0-108">权限</span><span class="sxs-lookup"><span data-stu-id="9fba0-108">Permissions</span></span>

<span data-ttu-id="9fba0-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9fba0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9fba0-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9fba0-111">Permission type</span></span>      | <span data-ttu-id="9fba0-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9fba0-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9fba0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9fba0-113">Delegated (work or school account)</span></span> | <span data-ttu-id="9fba0-114">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="9fba0-114">Mail.Send</span></span>    |
|<span data-ttu-id="9fba0-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9fba0-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9fba0-116">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="9fba0-116">Mail.Send</span></span>    |
|<span data-ttu-id="9fba0-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9fba0-117">Application</span></span> | <span data-ttu-id="9fba0-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="9fba0-118">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="9fba0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9fba0-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/send
POST /users/{id | userPrincipalName}/messages/{id}/send
```

## <a name="request-headers"></a><span data-ttu-id="9fba0-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9fba0-120">Request headers</span></span>

| <span data-ttu-id="9fba0-121">名称</span><span class="sxs-lookup"><span data-stu-id="9fba0-121">Name</span></span>       | <span data-ttu-id="9fba0-122">类型</span><span class="sxs-lookup"><span data-stu-id="9fba0-122">Type</span></span> | <span data-ttu-id="9fba0-123">说明</span><span class="sxs-lookup"><span data-stu-id="9fba0-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9fba0-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="9fba0-124">Authorization</span></span>  | <span data-ttu-id="9fba0-125">string</span><span class="sxs-lookup"><span data-stu-id="9fba0-125">string</span></span>  | <span data-ttu-id="9fba0-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9fba0-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9fba0-128">Content-Length</span><span class="sxs-lookup"><span data-stu-id="9fba0-128">Content-Length</span></span> | <span data-ttu-id="9fba0-129">数字</span><span class="sxs-lookup"><span data-stu-id="9fba0-129">number</span></span> | <span data-ttu-id="9fba0-130">0。 被必需。</span><span class="sxs-lookup"><span data-stu-id="9fba0-130">0. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9fba0-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="9fba0-131">Request body</span></span>

## <a name="response"></a><span data-ttu-id="9fba0-132">响应</span><span class="sxs-lookup"><span data-stu-id="9fba0-132">Response</span></span>

<span data-ttu-id="9fba0-p105">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="9fba0-p105">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9fba0-135">示例</span><span class="sxs-lookup"><span data-stu-id="9fba0-135">Example</span></span>

<span data-ttu-id="9fba0-136">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="9fba0-136">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="9fba0-137">请求</span><span class="sxs-lookup"><span data-stu-id="9fba0-137">Request</span></span>

<span data-ttu-id="9fba0-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9fba0-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_send"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/send
```

##### <a name="response"></a><span data-ttu-id="9fba0-139">响应</span><span class="sxs-lookup"><span data-stu-id="9fba0-139">Response</span></span>

<span data-ttu-id="9fba0-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="9fba0-140">Here is an example of the response.</span></span>
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
