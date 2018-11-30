---
title: 组：resetUnseenCount
description: 重置的上次访问后没有发现当前用户的所有帖子 unseenCount。 Office 365 组仅支持。
ms.openlocfilehash: b6218176f097759870aad4a3a2908759862002e2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048754"
---
# <a name="group-resetunseencount"></a><span data-ttu-id="96819-104">组：resetUnseenCount</span><span class="sxs-lookup"><span data-stu-id="96819-104">group: resetUnseenCount</span></span>

> <span data-ttu-id="96819-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="96819-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="96819-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="96819-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="96819-107">重置的上次访问后没有发现当前用户的所有帖子 unseenCount。</span><span class="sxs-lookup"><span data-stu-id="96819-107">Reset the unseenCount of all the posts that the current user has not seen since their last visit.</span></span> <span data-ttu-id="96819-108">Office 365 组仅支持。</span><span class="sxs-lookup"><span data-stu-id="96819-108">Supported for Office 365 Groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="96819-109">权限</span><span class="sxs-lookup"><span data-stu-id="96819-109">Permissions</span></span>
<span data-ttu-id="96819-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="96819-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96819-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="96819-112">Permission type</span></span>      | <span data-ttu-id="96819-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="96819-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="96819-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="96819-114">Delegated (work or school account)</span></span> | <span data-ttu-id="96819-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96819-115">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="96819-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="96819-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96819-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="96819-117">Not supported.</span></span>    |
|<span data-ttu-id="96819-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="96819-118">Application</span></span> | <span data-ttu-id="96819-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="96819-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="96819-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="96819-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/resetUnseenCount
```
## <a name="request-headers"></a><span data-ttu-id="96819-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="96819-121">Request headers</span></span>
| <span data-ttu-id="96819-122">标头</span><span class="sxs-lookup"><span data-stu-id="96819-122">Header</span></span>       | <span data-ttu-id="96819-123">值</span><span class="sxs-lookup"><span data-stu-id="96819-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="96819-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="96819-124">Authorization</span></span>  | <span data-ttu-id="96819-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="96819-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="96819-127">Prefer</span><span class="sxs-lookup"><span data-stu-id="96819-127">Prefer</span></span> | <span data-ttu-id="96819-128">return=minimal。</span><span class="sxs-lookup"><span data-stu-id="96819-128">return=minimal.</span></span> <span data-ttu-id="96819-129">如果 minimal 响应头包含在请求头中，那么成功响应返回 `204 No Content` 代码。</span><span class="sxs-lookup"><span data-stu-id="96819-129">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="96819-130">可选。</span><span class="sxs-lookup"><span data-stu-id="96819-130">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="96819-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="96819-131">Request body</span></span>
<span data-ttu-id="96819-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="96819-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96819-133">响应</span><span class="sxs-lookup"><span data-stu-id="96819-133">Response</span></span>
<span data-ttu-id="96819-p107">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="96819-p107">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96819-136">示例</span><span class="sxs-lookup"><span data-stu-id="96819-136">Example</span></span>
#### <a name="request"></a><span data-ttu-id="96819-137">请求</span><span class="sxs-lookup"><span data-stu-id="96819-137">Request</span></span>
<span data-ttu-id="96819-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="96819-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "group_resetunseencount"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/resetUnseenCount
```

#### <a name="response"></a><span data-ttu-id="96819-139">响应</span><span class="sxs-lookup"><span data-stu-id="96819-139">Response</span></span>
<span data-ttu-id="96819-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="96819-140">The following is an example of the response.</span></span> 
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
  "description": "group: resetUnseenCount",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
