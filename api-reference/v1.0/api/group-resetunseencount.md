---
title: 组：resetUnseenCount
description: 重置当前用户自上次访问后未查看的所有帖子的 unseenCount。 仅支持 Microsoft 365 组。
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 0f2880fb630675c31b107a10926754602ae1f8ce
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48041993"
---
# <a name="group-resetunseencount"></a><span data-ttu-id="e5682-104">组：resetUnseenCount</span><span class="sxs-lookup"><span data-stu-id="e5682-104">group: resetUnseenCount</span></span>

<span data-ttu-id="e5682-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e5682-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e5682-106">重置当前用户自上次访问后未查看的所有帖子的 unseenCount。</span><span class="sxs-lookup"><span data-stu-id="e5682-106">Reset the unseenCount of all the posts that the current user has not seen since their last visit.</span></span> <span data-ttu-id="e5682-107">仅支持 Microsoft 365 组。</span><span class="sxs-lookup"><span data-stu-id="e5682-107">Supported for Microsoft 365 groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="e5682-108">权限</span><span class="sxs-lookup"><span data-stu-id="e5682-108">Permissions</span></span>
<span data-ttu-id="e5682-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e5682-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5682-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e5682-111">Permission type</span></span>      | <span data-ttu-id="e5682-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e5682-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e5682-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e5682-113">Delegated (work or school account)</span></span> | <span data-ttu-id="e5682-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5682-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e5682-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e5682-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5682-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e5682-116">Not supported.</span></span>    |
|<span data-ttu-id="e5682-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e5682-117">Application</span></span> | <span data-ttu-id="e5682-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="e5682-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e5682-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e5682-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/resetUnseenCount
```
## <a name="request-headers"></a><span data-ttu-id="e5682-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e5682-120">Request headers</span></span>
| <span data-ttu-id="e5682-121">标头</span><span class="sxs-lookup"><span data-stu-id="e5682-121">Header</span></span>       | <span data-ttu-id="e5682-122">值</span><span class="sxs-lookup"><span data-stu-id="e5682-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e5682-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5682-123">Authorization</span></span>  | <span data-ttu-id="e5682-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e5682-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e5682-126">Prefer</span><span class="sxs-lookup"><span data-stu-id="e5682-126">Prefer</span></span> | <span data-ttu-id="e5682-127">return=minimal。</span><span class="sxs-lookup"><span data-stu-id="e5682-127">return=minimal.</span></span> <span data-ttu-id="e5682-128">如果 minimal 响应头包含在请求头中，那么成功响应返回 `204 No Content` 代码。</span><span class="sxs-lookup"><span data-stu-id="e5682-128">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="e5682-129">可选。</span><span class="sxs-lookup"><span data-stu-id="e5682-129">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="e5682-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="e5682-130">Request body</span></span>
<span data-ttu-id="e5682-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e5682-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e5682-132">响应</span><span class="sxs-lookup"><span data-stu-id="e5682-132">Response</span></span>
<span data-ttu-id="e5682-p106">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="e5682-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5682-135">示例</span><span class="sxs-lookup"><span data-stu-id="e5682-135">Example</span></span>
#### <a name="request"></a><span data-ttu-id="e5682-136">请求</span><span class="sxs-lookup"><span data-stu-id="e5682-136">Request</span></span>
<span data-ttu-id="e5682-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e5682-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e5682-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="e5682-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_resetunseencount"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/resetUnseenCount
```
# <a name="c"></a>[<span data-ttu-id="e5682-139">C#</span><span class="sxs-lookup"><span data-stu-id="e5682-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-resetunseencount-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e5682-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e5682-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-resetunseencount-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e5682-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e5682-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-resetunseencount-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e5682-142">Java</span><span class="sxs-lookup"><span data-stu-id="e5682-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-resetunseencount-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e5682-143">响应</span><span class="sxs-lookup"><span data-stu-id="e5682-143">Response</span></span>
<span data-ttu-id="e5682-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e5682-144">The following is an example of the response.</span></span> 
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
  "tocPath": "",
  "suppressions": [
  ]
}-->

