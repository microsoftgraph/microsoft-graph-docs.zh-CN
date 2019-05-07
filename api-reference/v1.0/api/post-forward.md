---
title: 帖子：转发
description: '将帖子转发给收件人。 您可以在请求中同时指定父对话和线程, '
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 65e8869774fe6823ae09349cf92627920d965f94
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33608560"
---
# <a name="post-forward"></a><span data-ttu-id="a4486-104">帖子：转发</span><span class="sxs-lookup"><span data-stu-id="a4486-104">post: forward</span></span>

<span data-ttu-id="a4486-p102">将帖子转发给收件人。可以在请求中同时指定父对话和线程，或者仅指定父线程，而不指定父对话。</span><span class="sxs-lookup"><span data-stu-id="a4486-p102">Forward a post to a recipient. You can specify both the parent conversation and thread in the request, or, you can specify just the parent thread without the parent conversation.</span></span> 

## <a name="permissions"></a><span data-ttu-id="a4486-107">权限</span><span class="sxs-lookup"><span data-stu-id="a4486-107">Permissions</span></span>
<span data-ttu-id="a4486-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a4486-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a4486-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a4486-110">Permission type</span></span>      | <span data-ttu-id="a4486-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a4486-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a4486-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a4486-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a4486-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4486-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a4486-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a4486-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a4486-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a4486-115">Not supported.</span></span>    |
|<span data-ttu-id="a4486-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a4486-116">Application</span></span> | <span data-ttu-id="a4486-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4486-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a4486-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a4486-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/posts/{id}/forward
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/forward

```
## <a name="request-headers"></a><span data-ttu-id="a4486-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a4486-119">Request headers</span></span>
| <span data-ttu-id="a4486-120">标头</span><span class="sxs-lookup"><span data-stu-id="a4486-120">Header</span></span>       | <span data-ttu-id="a4486-121">值</span><span class="sxs-lookup"><span data-stu-id="a4486-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a4486-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4486-122">Authorization</span></span>  | <span data-ttu-id="a4486-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a4486-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a4486-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="a4486-125">Request body</span></span>
<span data-ttu-id="a4486-126">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="a4486-126">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a4486-127">参数</span><span class="sxs-lookup"><span data-stu-id="a4486-127">Parameter</span></span>    | <span data-ttu-id="a4486-128">类型</span><span class="sxs-lookup"><span data-stu-id="a4486-128">Type</span></span>   |<span data-ttu-id="a4486-129">说明</span><span class="sxs-lookup"><span data-stu-id="a4486-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a4486-130">注释</span><span class="sxs-lookup"><span data-stu-id="a4486-130">comment</span></span>|<span data-ttu-id="a4486-131">String</span><span class="sxs-lookup"><span data-stu-id="a4486-131">String</span></span>|<span data-ttu-id="a4486-132">与帖子一起转发的可选注释。</span><span class="sxs-lookup"><span data-stu-id="a4486-132">Optional comment that is forwarded together with the post.</span></span>|
|<span data-ttu-id="a4486-133">toRecipients</span><span class="sxs-lookup"><span data-stu-id="a4486-133">toRecipients</span></span>|<span data-ttu-id="a4486-134">[recipient](../resources/recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="a4486-134">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="a4486-135">线程要转发至的收件人。</span><span class="sxs-lookup"><span data-stu-id="a4486-135">The recipients to whom the threaded is forwarded to.</span></span>|

## <a name="response"></a><span data-ttu-id="a4486-136">响应</span><span class="sxs-lookup"><span data-stu-id="a4486-136">Response</span></span>

<span data-ttu-id="a4486-p105">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="a4486-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4486-139">示例</span><span class="sxs-lookup"><span data-stu-id="a4486-139">Example</span></span>
<span data-ttu-id="a4486-140">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="a4486-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a4486-141">请求</span><span class="sxs-lookup"><span data-stu-id="a4486-141">Request</span></span>
<span data-ttu-id="a4486-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a4486-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "post_forward"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/threads/{id}/posts/{id}/forward
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

##### <a name="response"></a><span data-ttu-id="a4486-143">响应</span><span class="sxs-lookup"><span data-stu-id="a4486-143">Response</span></span>
<span data-ttu-id="a4486-144">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a4486-144">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="a4486-145">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="a4486-145">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a4486-146">语言</span><span class="sxs-lookup"><span data-stu-id="a4486-146">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/post_forward-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a4486-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="a4486-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/post_forward-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "post: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/post-forward.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/post-forward.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
