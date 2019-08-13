---
title: 邮件：发送
description: 在草稿箱文件夹中发送邮件。 邮件草稿可以是新邮件草稿、答复草稿、全部答复草稿或
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: fa51f2e658d399b45e66917151c88846b29205ee
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36346853"
---
# <a name="message-send"></a><span data-ttu-id="17749-104">邮件：发送</span><span class="sxs-lookup"><span data-stu-id="17749-104">message: send</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="17749-p102">在草稿箱文件夹中发送邮件。邮件草稿可以是新邮件草稿、答复草稿、全部答复草稿或转发草稿。然后邮件保存在已发送邮件文件夹中。</span><span class="sxs-lookup"><span data-stu-id="17749-p102">Send a message in the draft folder. The draft message can be a new message draft, reply draft, reply-all draft, or a forward draft. The message is then saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="17749-108">权限</span><span class="sxs-lookup"><span data-stu-id="17749-108">Permissions</span></span>

<span data-ttu-id="17749-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="17749-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17749-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="17749-111">Permission type</span></span>      | <span data-ttu-id="17749-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="17749-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="17749-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="17749-113">Delegated (work or school account)</span></span> | <span data-ttu-id="17749-114">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="17749-114">Mail.Send</span></span>    |
|<span data-ttu-id="17749-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="17749-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="17749-116">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="17749-116">Mail.Send</span></span>    |
|<span data-ttu-id="17749-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="17749-117">Application</span></span> | <span data-ttu-id="17749-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="17749-118">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="17749-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="17749-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/send
POST /users/{id | userPrincipalName}/messages/{id}/send
```

## <a name="request-headers"></a><span data-ttu-id="17749-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="17749-120">Request headers</span></span>

| <span data-ttu-id="17749-121">名称</span><span class="sxs-lookup"><span data-stu-id="17749-121">Name</span></span>       | <span data-ttu-id="17749-122">类型</span><span class="sxs-lookup"><span data-stu-id="17749-122">Type</span></span> | <span data-ttu-id="17749-123">说明</span><span class="sxs-lookup"><span data-stu-id="17749-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="17749-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="17749-124">Authorization</span></span>  | <span data-ttu-id="17749-125">string</span><span class="sxs-lookup"><span data-stu-id="17749-125">string</span></span>  | <span data-ttu-id="17749-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="17749-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="17749-128">Content-Length</span><span class="sxs-lookup"><span data-stu-id="17749-128">Content-Length</span></span> | <span data-ttu-id="17749-129">number</span><span class="sxs-lookup"><span data-stu-id="17749-129">number</span></span> | <span data-ttu-id="17749-130">0。必需。</span><span class="sxs-lookup"><span data-stu-id="17749-130">0. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="17749-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="17749-131">Request body</span></span>

## <a name="response"></a><span data-ttu-id="17749-132">响应</span><span class="sxs-lookup"><span data-stu-id="17749-132">Response</span></span>

<span data-ttu-id="17749-p105">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="17749-p105">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17749-135">示例</span><span class="sxs-lookup"><span data-stu-id="17749-135">Example</span></span>

<span data-ttu-id="17749-136">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="17749-136">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="17749-137">请求</span><span class="sxs-lookup"><span data-stu-id="17749-137">Request</span></span>

<span data-ttu-id="17749-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="17749-138">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="17749-139">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="17749-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_send"
}-->

```http
POST https://graph.microsoft.com/beta/me/messages/{id}/send
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="17749-140">C#</span><span class="sxs-lookup"><span data-stu-id="17749-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-send-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="17749-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="17749-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-send-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="17749-142">目标-C</span><span class="sxs-lookup"><span data-stu-id="17749-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-send-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="17749-143">Java</span><span class="sxs-lookup"><span data-stu-id="17749-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/message-send-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="17749-144">响应</span><span class="sxs-lookup"><span data-stu-id="17749-144">Response</span></span>

<span data-ttu-id="17749-145">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="17749-145">Here is an example of the response.</span></span>
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
