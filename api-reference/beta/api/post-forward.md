---
title: 帖子：转发
description: '将帖子转发给收件人。 您可以在请求中，指定的父对话和线程 '
localization_priority: Normal
ms.openlocfilehash: 64b7d87745cf897ea827d37a9cd4f4c60d197068
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889437"
---
# <a name="post-forward"></a><span data-ttu-id="681e6-104">帖子：转发</span><span class="sxs-lookup"><span data-stu-id="681e6-104">post: forward</span></span>

> <span data-ttu-id="681e6-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="681e6-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="681e6-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="681e6-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="681e6-p103">将帖子转发给收件人。可以在请求中同时指定父对话和线程，或者仅指定父线程，而不指定父对话。</span><span class="sxs-lookup"><span data-stu-id="681e6-p103">Forward a post to a recipient. You can specify both the parent conversation and thread in the request, or, you can specify just the parent thread without the parent conversation.</span></span> 

## <a name="permissions"></a><span data-ttu-id="681e6-109">权限</span><span class="sxs-lookup"><span data-stu-id="681e6-109">Permissions</span></span>
<span data-ttu-id="681e6-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="681e6-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="681e6-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="681e6-112">Permission type</span></span>      | <span data-ttu-id="681e6-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="681e6-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="681e6-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="681e6-114">Delegated (work or school account)</span></span> | <span data-ttu-id="681e6-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="681e6-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="681e6-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="681e6-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="681e6-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="681e6-117">Not supported.</span></span>    |
|<span data-ttu-id="681e6-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="681e6-118">Application</span></span> | <span data-ttu-id="681e6-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="681e6-119">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="681e6-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="681e6-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/posts/{id}/forward
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/forward

```
## <a name="request-headers"></a><span data-ttu-id="681e6-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="681e6-121">Request headers</span></span>
| <span data-ttu-id="681e6-122">标头</span><span class="sxs-lookup"><span data-stu-id="681e6-122">Header</span></span>       | <span data-ttu-id="681e6-123">值</span><span class="sxs-lookup"><span data-stu-id="681e6-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="681e6-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="681e6-124">Authorization</span></span>  | <span data-ttu-id="681e6-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="681e6-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="681e6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="681e6-127">Request body</span></span>
<span data-ttu-id="681e6-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="681e6-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="681e6-129">参数</span><span class="sxs-lookup"><span data-stu-id="681e6-129">Parameter</span></span>    | <span data-ttu-id="681e6-130">类型</span><span class="sxs-lookup"><span data-stu-id="681e6-130">Type</span></span>   |<span data-ttu-id="681e6-131">说明</span><span class="sxs-lookup"><span data-stu-id="681e6-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="681e6-132">注释</span><span class="sxs-lookup"><span data-stu-id="681e6-132">comment</span></span>|<span data-ttu-id="681e6-133">String</span><span class="sxs-lookup"><span data-stu-id="681e6-133">String</span></span>|<span data-ttu-id="681e6-134">与帖子一起转发的可选注释。</span><span class="sxs-lookup"><span data-stu-id="681e6-134">Optional comment that is forwarded together with the post.</span></span>|
|<span data-ttu-id="681e6-135">toRecipients</span><span class="sxs-lookup"><span data-stu-id="681e6-135">toRecipients</span></span>|<span data-ttu-id="681e6-136">[收件人](../resources/recipient.md) 集合</span><span class="sxs-lookup"><span data-stu-id="681e6-136">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="681e6-137">线程要转发至的收件人。</span><span class="sxs-lookup"><span data-stu-id="681e6-137">The recipients to whom the threaded is forwarded to.</span></span>|

## <a name="response"></a><span data-ttu-id="681e6-138">响应</span><span class="sxs-lookup"><span data-stu-id="681e6-138">Response</span></span>

<span data-ttu-id="681e6-p106">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="681e6-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="681e6-141">示例</span><span class="sxs-lookup"><span data-stu-id="681e6-141">Example</span></span>
<span data-ttu-id="681e6-142">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="681e6-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="681e6-143">请求</span><span class="sxs-lookup"><span data-stu-id="681e6-143">Request</span></span>
<span data-ttu-id="681e6-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="681e6-144">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="681e6-145">响应</span><span class="sxs-lookup"><span data-stu-id="681e6-145">Response</span></span>
<span data-ttu-id="681e6-146">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="681e6-146">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "post: forward",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
