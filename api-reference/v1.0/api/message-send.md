---
title: 邮件：发送
description: 在草稿箱文件夹中发送邮件。 邮件草稿可以是新邮件草稿、答复草稿、全部答复草稿或
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 0e81ff66a280e32f8224a471bd1dfd1d36e2e818
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42511479"
---
# <a name="message-send"></a><span data-ttu-id="b8ee0-104">邮件：发送</span><span class="sxs-lookup"><span data-stu-id="b8ee0-104">message: send</span></span>

<span data-ttu-id="b8ee0-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b8ee0-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b8ee0-p102">在草稿箱文件夹中发送邮件。邮件草稿可以是新邮件草稿、答复草稿、全部答复草稿或转发草稿。然后邮件保存在已发送邮件文件夹中。</span><span class="sxs-lookup"><span data-stu-id="b8ee0-p102">Send a message in the draft folder. The draft message can be a new message draft, reply draft, reply-all draft, or a forward draft. The message is then saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="b8ee0-109">权限</span><span class="sxs-lookup"><span data-stu-id="b8ee0-109">Permissions</span></span>

<span data-ttu-id="b8ee0-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b8ee0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8ee0-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="b8ee0-112">Permission type</span></span>      | <span data-ttu-id="b8ee0-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b8ee0-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b8ee0-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b8ee0-114">Delegated (work or school account)</span></span> | <span data-ttu-id="b8ee0-115">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="b8ee0-115">Mail.Send</span></span>    |
|<span data-ttu-id="b8ee0-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b8ee0-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b8ee0-117">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="b8ee0-117">Mail.Send</span></span>    |
|<span data-ttu-id="b8ee0-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="b8ee0-118">Application</span></span> | <span data-ttu-id="b8ee0-119">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="b8ee0-119">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="b8ee0-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b8ee0-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/send
POST /users/{id | userPrincipalName}/messages/{id}/send
```

## <a name="request-headers"></a><span data-ttu-id="b8ee0-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="b8ee0-121">Request headers</span></span>

| <span data-ttu-id="b8ee0-122">名称</span><span class="sxs-lookup"><span data-stu-id="b8ee0-122">Name</span></span>       | <span data-ttu-id="b8ee0-123">类型</span><span class="sxs-lookup"><span data-stu-id="b8ee0-123">Type</span></span> | <span data-ttu-id="b8ee0-124">说明</span><span class="sxs-lookup"><span data-stu-id="b8ee0-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b8ee0-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="b8ee0-125">Authorization</span></span>  | <span data-ttu-id="b8ee0-126">string</span><span class="sxs-lookup"><span data-stu-id="b8ee0-126">string</span></span>  | <span data-ttu-id="b8ee0-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b8ee0-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b8ee0-129">Content-Length</span><span class="sxs-lookup"><span data-stu-id="b8ee0-129">Content-Length</span></span> | <span data-ttu-id="b8ee0-130">number</span><span class="sxs-lookup"><span data-stu-id="b8ee0-130">number</span></span> | <span data-ttu-id="b8ee0-131">0。必需。</span><span class="sxs-lookup"><span data-stu-id="b8ee0-131">0. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b8ee0-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="b8ee0-132">Request body</span></span>

## <a name="response"></a><span data-ttu-id="b8ee0-133">响应</span><span class="sxs-lookup"><span data-stu-id="b8ee0-133">Response</span></span>

<span data-ttu-id="b8ee0-p105">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="b8ee0-p105">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8ee0-136">示例</span><span class="sxs-lookup"><span data-stu-id="b8ee0-136">Example</span></span>

<span data-ttu-id="b8ee0-137">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="b8ee0-137">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="b8ee0-138">请求</span><span class="sxs-lookup"><span data-stu-id="b8ee0-138">Request</span></span>

<span data-ttu-id="b8ee0-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b8ee0-139">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b8ee0-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="b8ee0-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_send"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/send
```
# <a name="c"></a>[<span data-ttu-id="b8ee0-141">C#</span><span class="sxs-lookup"><span data-stu-id="b8ee0-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-send-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b8ee0-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b8ee0-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-send-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b8ee0-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b8ee0-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-send-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b8ee0-144">Java</span><span class="sxs-lookup"><span data-stu-id="b8ee0-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-send-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b8ee0-145">响应</span><span class="sxs-lookup"><span data-stu-id="b8ee0-145">Response</span></span>

<span data-ttu-id="b8ee0-146">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="b8ee0-146">Here is an example of the response.</span></span>
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
