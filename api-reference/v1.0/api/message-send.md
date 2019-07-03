---
title: 邮件：发送
description: 在草稿箱文件夹中发送邮件。 邮件草稿可以是新邮件草稿、答复草稿、全部答复草稿或
localization_priority: Priority
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 4a2c1b59c95004c23d7a00426406d6a69a12b841
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35455278"
---
# <a name="message-send"></a><span data-ttu-id="205ba-104">邮件：发送</span><span class="sxs-lookup"><span data-stu-id="205ba-104">message: send</span></span>

<span data-ttu-id="205ba-p102">在草稿箱文件夹中发送邮件。邮件草稿可以是新邮件草稿、答复草稿、全部答复草稿或转发草稿。然后邮件保存在已发送邮件文件夹中。</span><span class="sxs-lookup"><span data-stu-id="205ba-p102">Send a message in the draft folder. The draft message can be a new message draft, reply draft, reply-all draft, or a forward draft. The message is then saved in the Sent Items folder.</span></span>

## <a name="permissions"></a><span data-ttu-id="205ba-108">权限</span><span class="sxs-lookup"><span data-stu-id="205ba-108">Permissions</span></span>

<span data-ttu-id="205ba-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="205ba-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="205ba-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="205ba-111">Permission type</span></span>      | <span data-ttu-id="205ba-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="205ba-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="205ba-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="205ba-113">Delegated (work or school account)</span></span> | <span data-ttu-id="205ba-114">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="205ba-114">Mail.Send</span></span>    |
|<span data-ttu-id="205ba-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="205ba-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="205ba-116">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="205ba-116">Mail.Send</span></span>    |
|<span data-ttu-id="205ba-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="205ba-117">Application</span></span> | <span data-ttu-id="205ba-118">Mail.Send</span><span class="sxs-lookup"><span data-stu-id="205ba-118">Mail.Send</span></span> |

## <a name="http-request"></a><span data-ttu-id="205ba-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="205ba-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /me/messages/{id}/send
POST /users/{id | userPrincipalName}/messages/{id}/send
```

## <a name="request-headers"></a><span data-ttu-id="205ba-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="205ba-120">Request headers</span></span>

| <span data-ttu-id="205ba-121">名称</span><span class="sxs-lookup"><span data-stu-id="205ba-121">Name</span></span>       | <span data-ttu-id="205ba-122">类型</span><span class="sxs-lookup"><span data-stu-id="205ba-122">Type</span></span> | <span data-ttu-id="205ba-123">说明</span><span class="sxs-lookup"><span data-stu-id="205ba-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="205ba-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="205ba-124">Authorization</span></span>  | <span data-ttu-id="205ba-125">string</span><span class="sxs-lookup"><span data-stu-id="205ba-125">string</span></span>  | <span data-ttu-id="205ba-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="205ba-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="205ba-128">Content-Length</span><span class="sxs-lookup"><span data-stu-id="205ba-128">Content-Length</span></span> | <span data-ttu-id="205ba-129">number</span><span class="sxs-lookup"><span data-stu-id="205ba-129">number</span></span> | <span data-ttu-id="205ba-130">0。必需。</span><span class="sxs-lookup"><span data-stu-id="205ba-130">0. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="205ba-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="205ba-131">Request body</span></span>

## <a name="response"></a><span data-ttu-id="205ba-132">响应</span><span class="sxs-lookup"><span data-stu-id="205ba-132">Response</span></span>

<span data-ttu-id="205ba-p105">如果成功，此方法返回 `202 Accepted` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="205ba-p105">If successful, this method returns `202 Accepted` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="205ba-135">示例</span><span class="sxs-lookup"><span data-stu-id="205ba-135">Example</span></span>

<span data-ttu-id="205ba-136">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="205ba-136">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="205ba-137">请求</span><span class="sxs-lookup"><span data-stu-id="205ba-137">Request</span></span>

<span data-ttu-id="205ba-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="205ba-138">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="205ba-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="205ba-139">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "message_send"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/messages/{id}/send
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="205ba-140">C#</span><span class="sxs-lookup"><span data-stu-id="205ba-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/message-send-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="205ba-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="205ba-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/message-send-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="205ba-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="205ba-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/message-send-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="205ba-143">响应</span><span class="sxs-lookup"><span data-stu-id="205ba-143">Response</span></span>

<span data-ttu-id="205ba-144">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="205ba-144">Here is an example of the response.</span></span>
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
