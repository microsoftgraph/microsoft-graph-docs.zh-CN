---
title: 组：resetUnseenCount
description: 重置当前用户自上次访问后未查看的所有帖子的 unseenCount。 仅支持 Microsoft 365 组。
author: yyuank
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 3858d98b6ae932043f3ba478f06be9d0e419dd4f
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897132"
---
# <a name="group-resetunseencount"></a><span data-ttu-id="90754-104">组：resetUnseenCount</span><span class="sxs-lookup"><span data-stu-id="90754-104">group: resetUnseenCount</span></span>

<span data-ttu-id="90754-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90754-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="90754-106">重置当前用户自上次访问后未查看的所有帖子的 unseenCount。</span><span class="sxs-lookup"><span data-stu-id="90754-106">Reset the unseenCount of all the posts that the current user has not seen since their last visit.</span></span> <span data-ttu-id="90754-107">仅支持 Microsoft 365 组。</span><span class="sxs-lookup"><span data-stu-id="90754-107">Supported for Microsoft 365 groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="90754-108">权限</span><span class="sxs-lookup"><span data-stu-id="90754-108">Permissions</span></span>
<span data-ttu-id="90754-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="90754-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90754-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="90754-111">Permission type</span></span>      | <span data-ttu-id="90754-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="90754-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="90754-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="90754-113">Delegated (work or school account)</span></span> | <span data-ttu-id="90754-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90754-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="90754-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="90754-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90754-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="90754-116">Not supported.</span></span>    |
|<span data-ttu-id="90754-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="90754-117">Application</span></span> | <span data-ttu-id="90754-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="90754-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="90754-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="90754-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/resetUnseenCount
```
## <a name="request-headers"></a><span data-ttu-id="90754-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="90754-120">Request headers</span></span>
| <span data-ttu-id="90754-121">标头</span><span class="sxs-lookup"><span data-stu-id="90754-121">Header</span></span>       | <span data-ttu-id="90754-122">值</span><span class="sxs-lookup"><span data-stu-id="90754-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="90754-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="90754-123">Authorization</span></span>  | <span data-ttu-id="90754-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="90754-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="90754-126">Prefer</span><span class="sxs-lookup"><span data-stu-id="90754-126">Prefer</span></span> | <span data-ttu-id="90754-127">return=minimal。</span><span class="sxs-lookup"><span data-stu-id="90754-127">return=minimal.</span></span> <span data-ttu-id="90754-128">如果 minimal 响应头包含在请求头中，那么成功响应返回 `204 No Content` 代码。</span><span class="sxs-lookup"><span data-stu-id="90754-128">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="90754-129">可选。</span><span class="sxs-lookup"><span data-stu-id="90754-129">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="90754-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="90754-130">Request body</span></span>
<span data-ttu-id="90754-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="90754-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90754-132">响应</span><span class="sxs-lookup"><span data-stu-id="90754-132">Response</span></span>
<span data-ttu-id="90754-p106">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="90754-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90754-135">示例</span><span class="sxs-lookup"><span data-stu-id="90754-135">Example</span></span>
#### <a name="request"></a><span data-ttu-id="90754-136">请求</span><span class="sxs-lookup"><span data-stu-id="90754-136">Request</span></span>
<span data-ttu-id="90754-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="90754-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="90754-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="90754-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_resetunseencount"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/resetUnseenCount
```
# <a name="c"></a>[<span data-ttu-id="90754-139">C#</span><span class="sxs-lookup"><span data-stu-id="90754-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-resetunseencount-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="90754-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="90754-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-resetunseencount-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="90754-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="90754-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-resetunseencount-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="90754-142">Java</span><span class="sxs-lookup"><span data-stu-id="90754-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-resetunseencount-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="90754-143">响应</span><span class="sxs-lookup"><span data-stu-id="90754-143">Response</span></span>
<span data-ttu-id="90754-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="90754-144">The following is an example of the response.</span></span> 
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
