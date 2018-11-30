---
title: 帖子：转发
description: '将帖子转发给收件人。 您可以在请求中，指定的父对话和线程 '
ms.openlocfilehash: 736b23aaf90cb7e4af243129e52a014ae623b8f4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044583"
---
# <a name="post-forward"></a><span data-ttu-id="158ab-104">帖子：转发</span><span class="sxs-lookup"><span data-stu-id="158ab-104">post: forward</span></span>

> <span data-ttu-id="158ab-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="158ab-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="158ab-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="158ab-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="158ab-p103">将帖子转发给收件人。可以在请求中同时指定父对话和线程，或者仅指定父线程，而不指定父对话。</span><span class="sxs-lookup"><span data-stu-id="158ab-p103">Forward a post to a recipient. You can specify both the parent conversation and thread in the request, or, you can specify just the parent thread without the parent conversation.</span></span> 

## <a name="permissions"></a><span data-ttu-id="158ab-109">权限</span><span class="sxs-lookup"><span data-stu-id="158ab-109">Permissions</span></span>
<span data-ttu-id="158ab-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="158ab-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="158ab-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="158ab-112">Permission type</span></span>      | <span data-ttu-id="158ab-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="158ab-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="158ab-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="158ab-114">Delegated (work or school account)</span></span> | <span data-ttu-id="158ab-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="158ab-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="158ab-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="158ab-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="158ab-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="158ab-117">Not supported.</span></span>    |
|<span data-ttu-id="158ab-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="158ab-118">Application</span></span> | <span data-ttu-id="158ab-119">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="158ab-119">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="158ab-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="158ab-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/threads/{id}/posts/{id}/forward
POST /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/forward

```
## <a name="request-headers"></a><span data-ttu-id="158ab-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="158ab-121">Request headers</span></span>
| <span data-ttu-id="158ab-122">标头</span><span class="sxs-lookup"><span data-stu-id="158ab-122">Header</span></span>       | <span data-ttu-id="158ab-123">值</span><span class="sxs-lookup"><span data-stu-id="158ab-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="158ab-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="158ab-124">Authorization</span></span>  | <span data-ttu-id="158ab-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="158ab-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="158ab-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="158ab-127">Request body</span></span>
<span data-ttu-id="158ab-128">在请求正文中，提供具有以下参数的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="158ab-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="158ab-129">参数</span><span class="sxs-lookup"><span data-stu-id="158ab-129">Parameter</span></span>    | <span data-ttu-id="158ab-130">类型</span><span class="sxs-lookup"><span data-stu-id="158ab-130">Type</span></span>   |<span data-ttu-id="158ab-131">说明</span><span class="sxs-lookup"><span data-stu-id="158ab-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="158ab-132">注释</span><span class="sxs-lookup"><span data-stu-id="158ab-132">comment</span></span>|<span data-ttu-id="158ab-133">String</span><span class="sxs-lookup"><span data-stu-id="158ab-133">String</span></span>|<span data-ttu-id="158ab-134">与帖子一起转发的可选注释。</span><span class="sxs-lookup"><span data-stu-id="158ab-134">Optional comment that is forwarded together with the post.</span></span>|
|<span data-ttu-id="158ab-135">toRecipients</span><span class="sxs-lookup"><span data-stu-id="158ab-135">toRecipients</span></span>|<span data-ttu-id="158ab-136">[收件人](../resources/recipient.md) 集合</span><span class="sxs-lookup"><span data-stu-id="158ab-136">[recipient](../resources/recipient.md) collection</span></span>|<span data-ttu-id="158ab-137">线程要转发至的收件人。</span><span class="sxs-lookup"><span data-stu-id="158ab-137">The recipients to whom the threaded is forwarded to.</span></span>|

## <a name="response"></a><span data-ttu-id="158ab-138">响应</span><span class="sxs-lookup"><span data-stu-id="158ab-138">Response</span></span>

<span data-ttu-id="158ab-p106">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="158ab-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="158ab-141">示例</span><span class="sxs-lookup"><span data-stu-id="158ab-141">Example</span></span>
<span data-ttu-id="158ab-142">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="158ab-142">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="158ab-143">请求</span><span class="sxs-lookup"><span data-stu-id="158ab-143">Request</span></span>
<span data-ttu-id="158ab-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="158ab-144">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="158ab-145">响应</span><span class="sxs-lookup"><span data-stu-id="158ab-145">Response</span></span>
<span data-ttu-id="158ab-146">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="158ab-146">Here is an example of the response.</span></span>
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
