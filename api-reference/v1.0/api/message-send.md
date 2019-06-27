---
title: 邮件：发送
description: 在草稿箱文件夹中发送邮件。 邮件草稿可以是新邮件草稿、答复草稿、全部答复草稿或
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: acdec6ef1aeef6671108a72a1b31c709ac9f6a23
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35276767"
---
# <a name="message-send"></a><span data-ttu-id="24d0d-104">邮件：发送</span><span class="sxs-lookup"><span data-stu-id="24d0d-104">message: send</span></span>

<span data-ttu-id="24d0d-p102">在草稿箱文件夹中发送邮件。邮件草稿可以是新邮件草稿、答复草稿、全部答复草稿或转发草稿。然后邮件保存在已发送邮件文件夹中。</span><span class="sxs-lookup"><span data-stu-id="24d0d-p102">Send a message in the draft folder. The draft message can be a new message draft, reply draft, reply-all draft, or a forward draft. The message is then saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="24d0d-108">权限</span><span class="sxs-lookup"><span data-stu-id="24d0d-108">Permissions</span></span>

<span data-ttu-id="24d0d-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="24d0d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24d0d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="24d0d-111">Permission type</span></span>      | <span data-ttu-id="24d0d-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="24d0d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="24d0d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="24d0d-113">Delegated (work or school account)</span></span> | <span data-ttu-id="24d0d-114">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="24d0d-114">Mail.Send</span></span>    |
|<span data-ttu-id="24d0d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="24d0d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24d0d-116">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="24d0d-116">Mail.Send</span></span>    |
|<span data-ttu-id="24d0d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="24d0d-117">Application</span></span> | <span data-ttu-id="24d0d-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="24d0d-118">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="24d0d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="24d0d-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/send
POST /users/{id | userPrincipalName}/messages/{id}/send
```

## <a name="request-headers"></a><span data-ttu-id="24d0d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="24d0d-120">Request headers</span></span>

| <span data-ttu-id="24d0d-121">名称</span><span class="sxs-lookup"><span data-stu-id="24d0d-121">Name</span></span>       | <span data-ttu-id="24d0d-122">类型</span><span class="sxs-lookup"><span data-stu-id="24d0d-122">Type</span></span> | <span data-ttu-id="24d0d-123">说明</span><span class="sxs-lookup"><span data-stu-id="24d0d-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="24d0d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="24d0d-124">Authorization</span></span>  | <span data-ttu-id="24d0d-125">string</span><span class="sxs-lookup"><span data-stu-id="24d0d-125">string</span></span>  | <span data-ttu-id="24d0d-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="24d0d-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="24d0d-128">Content-Length</span><span class="sxs-lookup"><span data-stu-id="24d0d-128">Content-Length</span></span> | <span data-ttu-id="24d0d-129">number</span><span class="sxs-lookup"><span data-stu-id="24d0d-129">number</span></span> | <span data-ttu-id="24d0d-130">0。必需。</span><span class="sxs-lookup"><span data-stu-id="24d0d-130">0. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="24d0d-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="24d0d-131">Request body</span></span>

## <a name="response"></a><span data-ttu-id="24d0d-132">响应</span><span class="sxs-lookup"><span data-stu-id="24d0d-132">Response</span></span>

<span data-ttu-id="24d0d-p105">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="24d0d-p105">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24d0d-135">示例</span><span class="sxs-lookup"><span data-stu-id="24d0d-135">Example</span></span>

<span data-ttu-id="24d0d-136">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="24d0d-136">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="24d0d-137">请求</span><span class="sxs-lookup"><span data-stu-id="24d0d-137">Request</span></span>

<span data-ttu-id="24d0d-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="24d0d-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "message_send"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/send
```

##### <a name="response"></a><span data-ttu-id="24d0d-139">响应</span><span class="sxs-lookup"><span data-stu-id="24d0d-139">Response</span></span>

<span data-ttu-id="24d0d-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="24d0d-140">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 202 Accepted
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="24d0d-141">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="24d0d-141">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="24d0d-142">C#</span><span class="sxs-lookup"><span data-stu-id="24d0d-142">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/message_send-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="24d0d-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="24d0d-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/message_send-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="24d0d-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="24d0d-144">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/message_send-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "message: send",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/message-send.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/message-send.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/message-send.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
