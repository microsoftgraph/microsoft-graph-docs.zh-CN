---
title: 邮件：发送
description: 在草稿箱文件夹中发送邮件。 邮件草稿可以是新邮件草稿、答复草稿、全部答复草稿或
localization_priority: Normal
author: svpsiva
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 60441163dacebe8ca5b15e0571100c4b87f50ef7
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48976476"
---
# <a name="message-send"></a><span data-ttu-id="78599-104">邮件：发送</span><span class="sxs-lookup"><span data-stu-id="78599-104">message: send</span></span>

<span data-ttu-id="78599-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78599-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78599-p102">在草稿箱文件夹中发送邮件。邮件草稿可以是新邮件草稿、答复草稿、全部答复草稿或转发草稿。然后邮件保存在已发送邮件文件夹中。</span><span class="sxs-lookup"><span data-stu-id="78599-p102">Send a message in the draft folder. The draft message can be a new message draft, reply draft, reply-all draft, or a forward draft. The message is then saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="78599-109">权限</span><span class="sxs-lookup"><span data-stu-id="78599-109">Permissions</span></span>

<span data-ttu-id="78599-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="78599-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78599-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="78599-112">Permission type</span></span>      | <span data-ttu-id="78599-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="78599-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="78599-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="78599-114">Delegated (work or school account)</span></span> | <span data-ttu-id="78599-115">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="78599-115">Mail.Send</span></span>    |
|<span data-ttu-id="78599-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="78599-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="78599-117">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="78599-117">Mail.Send</span></span>    |
|<span data-ttu-id="78599-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="78599-118">Application</span></span> | <span data-ttu-id="78599-119">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="78599-119">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="78599-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="78599-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/send
POST /users/{id | userPrincipalName}/messages/{id}/send
```

## <a name="request-headers"></a><span data-ttu-id="78599-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="78599-121">Request headers</span></span>

| <span data-ttu-id="78599-122">名称</span><span class="sxs-lookup"><span data-stu-id="78599-122">Name</span></span>       | <span data-ttu-id="78599-123">类型</span><span class="sxs-lookup"><span data-stu-id="78599-123">Type</span></span> | <span data-ttu-id="78599-124">说明</span><span class="sxs-lookup"><span data-stu-id="78599-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="78599-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="78599-125">Authorization</span></span>  | <span data-ttu-id="78599-126">string</span><span class="sxs-lookup"><span data-stu-id="78599-126">string</span></span>  | <span data-ttu-id="78599-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="78599-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="78599-129">Content-Length</span><span class="sxs-lookup"><span data-stu-id="78599-129">Content-Length</span></span> | <span data-ttu-id="78599-130">number</span><span class="sxs-lookup"><span data-stu-id="78599-130">number</span></span> | <span data-ttu-id="78599-131">0。必需。</span><span class="sxs-lookup"><span data-stu-id="78599-131">0. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="78599-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="78599-132">Request body</span></span>

## <a name="response"></a><span data-ttu-id="78599-133">响应</span><span class="sxs-lookup"><span data-stu-id="78599-133">Response</span></span>

<span data-ttu-id="78599-p105">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="78599-p105">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78599-136">示例</span><span class="sxs-lookup"><span data-stu-id="78599-136">Example</span></span>

<span data-ttu-id="78599-137">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="78599-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="78599-138">请求</span><span class="sxs-lookup"><span data-stu-id="78599-138">Request</span></span>

<span data-ttu-id="78599-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="78599-139">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="78599-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="78599-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_send"
}-->

```http
POST https://graph.microsoft.com/beta/me/messages/{id}/send
```
# <a name="c"></a>[<span data-ttu-id="78599-141">C#</span><span class="sxs-lookup"><span data-stu-id="78599-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-send-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="78599-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="78599-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-send-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="78599-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="78599-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-send-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="78599-144">Java</span><span class="sxs-lookup"><span data-stu-id="78599-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-send-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="78599-145">响应</span><span class="sxs-lookup"><span data-stu-id="78599-145">Response</span></span>

<span data-ttu-id="78599-146">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="78599-146">Here is an example of the response.</span></span>
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
  "description": "message: send",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


