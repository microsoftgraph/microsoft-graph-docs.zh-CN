---
title: 邮件：发送
description: 发送现有草稿邮件。
localization_priority: Priority
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 8be54552df8acf7faa67c070e85f63f48a5c23d4
ms.sourcegitcommit: cec76c5a58b359d79df764c849c8b459349b3b52
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2021
ms.locfileid: "52645491"
---
# <a name="message-send"></a><span data-ttu-id="d5e62-103">邮件：发送</span><span class="sxs-lookup"><span data-stu-id="d5e62-103">message: send</span></span>

<span data-ttu-id="d5e62-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5e62-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d5e62-105">发送现有草稿邮件。</span><span class="sxs-lookup"><span data-stu-id="d5e62-105">Send an existing draft message.</span></span> 

<span data-ttu-id="d5e62-106">邮件草稿可以是新邮件[草稿](../api/user-post-messages.md)、[答复草稿](../api/message-createreply.md)、[全部答复草稿](../api/message-createreplyall.md)或[转发草稿](../api/message-createforward.md)。</span><span class="sxs-lookup"><span data-stu-id="d5e62-106">The draft message can be a new message [draft](../api/user-post-messages.md), [reply draft](../api/message-createreply.md), [reply-all draft](../api/message-createreplyall.md), or a [forward draft](../api/message-createforward.md).</span></span>

<span data-ttu-id="d5e62-107">此方法将邮件保存在 **“已发送邮件”** 文件夹中。</span><span class="sxs-lookup"><span data-stu-id="d5e62-107">This method saves the message in the **Sent Items** folder.</span></span>

<span data-ttu-id="d5e62-108">或者，通过一次操作[发送新消息](../api/user-sendmail.md)。</span><span class="sxs-lookup"><span data-stu-id="d5e62-108">Alternatively, [send a new message](../api/user-sendmail.md) in a single operation.</span></span>

## <a name="permissions"></a><span data-ttu-id="d5e62-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="d5e62-109">Permissions</span></span>
<span data-ttu-id="d5e62-p101">要调用此 API，需要以下权限。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d5e62-p101">One of the following permissions are required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d5e62-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="d5e62-112">Permission type</span></span>      | <span data-ttu-id="d5e62-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d5e62-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d5e62-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d5e62-114">Delegated (work or school account)</span></span> | <span data-ttu-id="d5e62-115">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="d5e62-115">Mail.Send</span></span>    |
|<span data-ttu-id="d5e62-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d5e62-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5e62-117">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="d5e62-117">Mail.Send</span></span>    |
|<span data-ttu-id="d5e62-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="d5e62-118">Application</span></span> | <span data-ttu-id="d5e62-119">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="d5e62-119">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="d5e62-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d5e62-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/send
POST /users/{id | userPrincipalName}/messages/{id}/send
```

## <a name="request-headers"></a><span data-ttu-id="d5e62-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="d5e62-121">Request headers</span></span>

| <span data-ttu-id="d5e62-122">名称</span><span class="sxs-lookup"><span data-stu-id="d5e62-122">Name</span></span>       | <span data-ttu-id="d5e62-123">类型</span><span class="sxs-lookup"><span data-stu-id="d5e62-123">Type</span></span> | <span data-ttu-id="d5e62-124">说明</span><span class="sxs-lookup"><span data-stu-id="d5e62-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d5e62-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5e62-125">Authorization</span></span>  | <span data-ttu-id="d5e62-126">string</span><span class="sxs-lookup"><span data-stu-id="d5e62-126">string</span></span>  | <span data-ttu-id="d5e62-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d5e62-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d5e62-129">Content-Length</span><span class="sxs-lookup"><span data-stu-id="d5e62-129">Content-Length</span></span> | <span data-ttu-id="d5e62-130">number</span><span class="sxs-lookup"><span data-stu-id="d5e62-130">number</span></span> | <span data-ttu-id="d5e62-131">0。必需。</span><span class="sxs-lookup"><span data-stu-id="d5e62-131">0. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d5e62-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="d5e62-132">Request body</span></span>
<span data-ttu-id="d5e62-133">由于此方法发送现有草稿邮件，因此不需要指定请求正文。</span><span class="sxs-lookup"><span data-stu-id="d5e62-133">Since this method sends an already existing draft message, specifying a request body is not necessary.</span></span>

## <a name="response"></a><span data-ttu-id="d5e62-134">响应</span><span class="sxs-lookup"><span data-stu-id="d5e62-134">Response</span></span>

<span data-ttu-id="d5e62-p103">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="d5e62-p103">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d5e62-137">示例</span><span class="sxs-lookup"><span data-stu-id="d5e62-137">Examples</span></span>

### <a name="example-1-send-an-existing-draft-message"></a><span data-ttu-id="d5e62-138">示例 1：发送现有草稿邮件</span><span class="sxs-lookup"><span data-stu-id="d5e62-138">Example 1: Send an existing draft message</span></span>

<span data-ttu-id="d5e62-139">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="d5e62-139">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="d5e62-140">请求</span><span class="sxs-lookup"><span data-stu-id="d5e62-140">Request</span></span>

<span data-ttu-id="d5e62-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d5e62-141">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="d5e62-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="d5e62-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_send"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/send
```
# <a name="c"></a>[<span data-ttu-id="d5e62-143">C#</span><span class="sxs-lookup"><span data-stu-id="d5e62-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-send-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d5e62-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d5e62-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-send-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d5e62-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d5e62-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-send-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d5e62-146">Java</span><span class="sxs-lookup"><span data-stu-id="d5e62-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-send-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d5e62-147">响应</span><span class="sxs-lookup"><span data-stu-id="d5e62-147">Response</span></span>

<span data-ttu-id="d5e62-148">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d5e62-148">Here is an example of the response.</span></span>
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
  "tocPath": "",
  "suppressions": [
  ]
}-->

