---
title: 帖子：转发
description: '将帖子转发给收件人。 您可以在请求中同时指定父对话和线程， '
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 2095e5a22ed15ff5444f424da475cda314925e37
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48980435"
---
# <a name="post-forward"></a><span data-ttu-id="7c997-104">帖子：转发</span><span class="sxs-lookup"><span data-stu-id="7c997-104">post: forward</span></span>

<span data-ttu-id="7c997-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c997-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c997-p102">将帖子转发给收件人。可以在请求中同时指定父对话和线程，或者仅指定父线程，而不指定父对话。</span><span class="sxs-lookup"><span data-stu-id="7c997-p102">Forward a post to a recipient. You can specify both the parent conversation and thread in the request, or, you can specify just the parent thread without the parent conversation.</span></span> 

## <a name="permissions"></a><span data-ttu-id="7c997-108">权限</span><span class="sxs-lookup"><span data-stu-id="7c997-108">Permissions</span></span>
<span data-ttu-id="7c997-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7c997-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c997-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7c997-111">Permission type</span></span>      | <span data-ttu-id="7c997-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7c997-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7c997-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7c997-113">Delegated (work or school account)</span></span> | <span data-ttu-id="7c997-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c997-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="7c997-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7c997-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7c997-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7c997-116">Not supported.</span></span>    |
|<span data-ttu-id="7c997-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7c997-117">Application</span></span> | <span data-ttu-id="7c997-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c997-118">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7c997-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7c997-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/posts/{id}/forward
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/forward

```
## <a name="request-headers"></a><span data-ttu-id="7c997-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7c997-120">Request headers</span></span>
| <span data-ttu-id="7c997-121">标头</span><span class="sxs-lookup"><span data-stu-id="7c997-121">Header</span></span>       | <span data-ttu-id="7c997-122">值</span><span class="sxs-lookup"><span data-stu-id="7c997-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7c997-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c997-123">Authorization</span></span>  | <span data-ttu-id="7c997-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7c997-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7c997-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="7c997-126">Request body</span></span>
<span data-ttu-id="7c997-127">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="7c997-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="7c997-128">参数</span><span class="sxs-lookup"><span data-stu-id="7c997-128">Parameter</span></span>    | <span data-ttu-id="7c997-129">类型</span><span class="sxs-lookup"><span data-stu-id="7c997-129">Type</span></span>   |<span data-ttu-id="7c997-130">说明</span><span class="sxs-lookup"><span data-stu-id="7c997-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7c997-131">注释</span><span class="sxs-lookup"><span data-stu-id="7c997-131">comment</span></span>|<span data-ttu-id="7c997-132">String</span><span class="sxs-lookup"><span data-stu-id="7c997-132">String</span></span>|<span data-ttu-id="7c997-133">与帖子一起转发的可选注释。</span><span class="sxs-lookup"><span data-stu-id="7c997-133">Optional comment that is forwarded together with the post.</span></span>|
|<span data-ttu-id="7c997-134">toRecipients</span><span class="sxs-lookup"><span data-stu-id="7c997-134">toRecipients</span></span>|<span data-ttu-id="7c997-135">[recipient](../resources/recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="7c997-135">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="7c997-136">线程要转发至的收件人。</span><span class="sxs-lookup"><span data-stu-id="7c997-136">The recipients to whom the threaded is forwarded to.</span></span>|

## <a name="response"></a><span data-ttu-id="7c997-137">响应</span><span class="sxs-lookup"><span data-stu-id="7c997-137">Response</span></span>

<span data-ttu-id="7c997-p105">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="7c997-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c997-140">示例</span><span class="sxs-lookup"><span data-stu-id="7c997-140">Example</span></span>
<span data-ttu-id="7c997-141">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="7c997-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7c997-142">请求</span><span class="sxs-lookup"><span data-stu-id="7c997-142">Request</span></span>
<span data-ttu-id="7c997-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7c997-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7c997-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="7c997-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_forward"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/threads/{id}/posts/{id}/forward
Content-type: application/json
Content-length: 166

{
  "comment": "comment-value",
  "toRecipients": [
    {
      "emailAddress": {
        "name": "name-value",
        "address": "address-value"
      }
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="7c997-145">C#</span><span class="sxs-lookup"><span data-stu-id="7c997-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-forward-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7c997-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7c997-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-forward-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7c997-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7c997-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-forward-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7c997-148">Java</span><span class="sxs-lookup"><span data-stu-id="7c997-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-forward-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7c997-149">响应</span><span class="sxs-lookup"><span data-stu-id="7c997-149">Response</span></span>
<span data-ttu-id="7c997-150">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="7c997-150">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "post: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


