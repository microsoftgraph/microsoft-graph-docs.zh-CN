---
title: 邮件：发送
description: 在草稿箱文件夹中发送邮件。 邮件草稿可以是新邮件草稿、答复草稿、全部答复草稿或
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 96ea8ccf3f44edb8c5b75b3e955d2381aa339d84
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131098"
---
# <a name="message-send"></a><span data-ttu-id="66023-104">邮件：发送</span><span class="sxs-lookup"><span data-stu-id="66023-104">message: send</span></span>

<span data-ttu-id="66023-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66023-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66023-p102">在草稿箱文件夹中发送邮件。邮件草稿可以是新邮件草稿、答复草稿、全部答复草稿或转发草稿。然后邮件保存在已发送邮件文件夹中。</span><span class="sxs-lookup"><span data-stu-id="66023-p102">Send a message in the draft folder. The draft message can be a new message draft, reply draft, reply-all draft, or a forward draft. The message is then saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="66023-109">权限</span><span class="sxs-lookup"><span data-stu-id="66023-109">Permissions</span></span>

<span data-ttu-id="66023-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="66023-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66023-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="66023-112">Permission type</span></span>      | <span data-ttu-id="66023-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="66023-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="66023-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="66023-114">Delegated (work or school account)</span></span> | <span data-ttu-id="66023-115">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="66023-115">Mail.Send</span></span>    |
|<span data-ttu-id="66023-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="66023-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66023-117">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="66023-117">Mail.Send</span></span>    |
|<span data-ttu-id="66023-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="66023-118">Application</span></span> | <span data-ttu-id="66023-119">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="66023-119">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="66023-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="66023-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/send
POST /users/{id | userPrincipalName}/messages/{id}/send
```

## <a name="request-headers"></a><span data-ttu-id="66023-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="66023-121">Request headers</span></span>

| <span data-ttu-id="66023-122">名称</span><span class="sxs-lookup"><span data-stu-id="66023-122">Name</span></span>       | <span data-ttu-id="66023-123">类型</span><span class="sxs-lookup"><span data-stu-id="66023-123">Type</span></span> | <span data-ttu-id="66023-124">说明</span><span class="sxs-lookup"><span data-stu-id="66023-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="66023-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="66023-125">Authorization</span></span>  | <span data-ttu-id="66023-126">string</span><span class="sxs-lookup"><span data-stu-id="66023-126">string</span></span>  | <span data-ttu-id="66023-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="66023-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="66023-129">Content-Length</span><span class="sxs-lookup"><span data-stu-id="66023-129">Content-Length</span></span> | <span data-ttu-id="66023-130">number</span><span class="sxs-lookup"><span data-stu-id="66023-130">number</span></span> | <span data-ttu-id="66023-131">0。必需。</span><span class="sxs-lookup"><span data-stu-id="66023-131">0. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="66023-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="66023-132">Request body</span></span>

## <a name="response"></a><span data-ttu-id="66023-133">响应</span><span class="sxs-lookup"><span data-stu-id="66023-133">Response</span></span>

<span data-ttu-id="66023-p105">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="66023-p105">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66023-136">示例</span><span class="sxs-lookup"><span data-stu-id="66023-136">Example</span></span>

<span data-ttu-id="66023-137">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="66023-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="66023-138">请求</span><span class="sxs-lookup"><span data-stu-id="66023-138">Request</span></span>

<span data-ttu-id="66023-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="66023-139">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="66023-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="66023-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_send"
}-->

```http
POST https://graph.microsoft.com/beta/me/messages/{id}/send
```
# <a name="c"></a>[<span data-ttu-id="66023-141">C#</span><span class="sxs-lookup"><span data-stu-id="66023-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-send-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="66023-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="66023-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-send-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="66023-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="66023-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-send-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="66023-144">Java</span><span class="sxs-lookup"><span data-stu-id="66023-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-send-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="66023-145">响应</span><span class="sxs-lookup"><span data-stu-id="66023-145">Response</span></span>

<span data-ttu-id="66023-146">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="66023-146">Here is an example of the response.</span></span>
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


