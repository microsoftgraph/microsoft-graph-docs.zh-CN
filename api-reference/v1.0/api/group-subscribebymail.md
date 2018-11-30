---
title: 组：subscribeByMail
description: 调用此方法将允许当前用户接收有关该组中新帖子、活动和文件的电子邮件通知。仅支持 Office 365 组。
ms.openlocfilehash: c075f11de44899b15873baa226a68767e776971e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008593"
---
# <a name="group-subscribebymail"></a><span data-ttu-id="7081a-104">组：subscribeByMail</span><span class="sxs-lookup"><span data-stu-id="7081a-104">group: subscribeByMail</span></span>
<span data-ttu-id="7081a-p102">调用此方法将允许当前用户接收有关该组中新帖子、活动和文件的电子邮件通知。仅支持 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="7081a-p102">Calling this method will enable the current user to receive email notifications for this group, about new posts, events, and files in that group. Supported for Office 365 groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="7081a-107">权限</span><span class="sxs-lookup"><span data-stu-id="7081a-107">Permissions</span></span>
<span data-ttu-id="7081a-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7081a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7081a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="7081a-110">Permission type</span></span>      | <span data-ttu-id="7081a-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7081a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7081a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7081a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7081a-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7081a-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="7081a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7081a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7081a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="7081a-115">Not supported.</span></span>    |
|<span data-ttu-id="7081a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="7081a-116">Application</span></span> | <span data-ttu-id="7081a-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="7081a-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7081a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7081a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/subscribeByMail
```
## <a name="request-headers"></a><span data-ttu-id="7081a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="7081a-119">Request headers</span></span>
| <span data-ttu-id="7081a-120">标头</span><span class="sxs-lookup"><span data-stu-id="7081a-120">Header</span></span>       | <span data-ttu-id="7081a-121">值</span><span class="sxs-lookup"><span data-stu-id="7081a-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7081a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7081a-122">Authorization</span></span>  | <span data-ttu-id="7081a-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7081a-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7081a-125">Prefer</span><span class="sxs-lookup"><span data-stu-id="7081a-125">Prefer</span></span> | <span data-ttu-id="7081a-126">return=minimal。</span><span class="sxs-lookup"><span data-stu-id="7081a-126">return=minimal.</span></span> <span data-ttu-id="7081a-127">如果 minimal 响应头包含在请求头中，那么成功响应返回 `204 No Content` 代码。</span><span class="sxs-lookup"><span data-stu-id="7081a-127">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="7081a-128">可选。</span><span class="sxs-lookup"><span data-stu-id="7081a-128">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="7081a-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="7081a-129">Request body</span></span>
<span data-ttu-id="7081a-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7081a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7081a-131">响应</span><span class="sxs-lookup"><span data-stu-id="7081a-131">Response</span></span>
<span data-ttu-id="7081a-p106">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="7081a-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7081a-134">示例</span><span class="sxs-lookup"><span data-stu-id="7081a-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="7081a-135">请求</span><span class="sxs-lookup"><span data-stu-id="7081a-135">Request</span></span>
<span data-ttu-id="7081a-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7081a-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_subscribebymail"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/subscribeByMail
```

#### <a name="response"></a><span data-ttu-id="7081a-137">响应</span><span class="sxs-lookup"><span data-stu-id="7081a-137">Response</span></span>
<span data-ttu-id="7081a-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7081a-138">The following is an example of the response.</span></span> 
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
  "description": "group: subscribeByMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->