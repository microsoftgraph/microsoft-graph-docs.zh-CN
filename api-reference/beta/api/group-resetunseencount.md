---
title: 组：resetUnseenCount
description: 重置当前用户自上次访问后未查看的所有帖子的 unseenCount。
author: Jordanndahl
localization_priority: Normal
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 8ca343a5d056f2fa673cc02030b2a94265fa24f1
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52681275"
---
# <a name="group-resetunseencount"></a><span data-ttu-id="b43b0-103">组：resetUnseenCount</span><span class="sxs-lookup"><span data-stu-id="b43b0-103">group: resetUnseenCount</span></span>

<span data-ttu-id="b43b0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b43b0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b43b0-105">重置当前用户自上次访问后未查看的所有帖子的 unseenCount。</span><span class="sxs-lookup"><span data-stu-id="b43b0-105">Reset the unseenCount of all the posts that the current user has not seen since their last visit.</span></span> <span data-ttu-id="b43b0-106">仅支持 Microsoft 365 组。</span><span class="sxs-lookup"><span data-stu-id="b43b0-106">Supported for Microsoft 365 groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="b43b0-107">权限</span><span class="sxs-lookup"><span data-stu-id="b43b0-107">Permissions</span></span>
<span data-ttu-id="b43b0-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b43b0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b43b0-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b43b0-110">Permission type</span></span>      | <span data-ttu-id="b43b0-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b43b0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b43b0-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b43b0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b43b0-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b43b0-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b43b0-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b43b0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b43b0-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b43b0-115">Not supported.</span></span>    |
|<span data-ttu-id="b43b0-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b43b0-116">Application</span></span> | <span data-ttu-id="b43b0-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="b43b0-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b43b0-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b43b0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/resetUnseenCount
```
## <a name="request-headers"></a><span data-ttu-id="b43b0-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b43b0-119">Request headers</span></span>
| <span data-ttu-id="b43b0-120">标头</span><span class="sxs-lookup"><span data-stu-id="b43b0-120">Header</span></span>       | <span data-ttu-id="b43b0-121">值</span><span class="sxs-lookup"><span data-stu-id="b43b0-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b43b0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b43b0-122">Authorization</span></span>  | <span data-ttu-id="b43b0-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b43b0-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b43b0-125">Prefer</span><span class="sxs-lookup"><span data-stu-id="b43b0-125">Prefer</span></span> | <span data-ttu-id="b43b0-126">return=minimal。</span><span class="sxs-lookup"><span data-stu-id="b43b0-126">return=minimal.</span></span> <span data-ttu-id="b43b0-127">如果 minimal 响应头包含在请求头中，那么成功响应返回 `204 No Content` 代码。</span><span class="sxs-lookup"><span data-stu-id="b43b0-127">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="b43b0-128">可选。</span><span class="sxs-lookup"><span data-stu-id="b43b0-128">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="b43b0-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="b43b0-129">Request body</span></span>
<span data-ttu-id="b43b0-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b43b0-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b43b0-131">响应</span><span class="sxs-lookup"><span data-stu-id="b43b0-131">Response</span></span>
<span data-ttu-id="b43b0-p105">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="b43b0-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b43b0-134">示例</span><span class="sxs-lookup"><span data-stu-id="b43b0-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="b43b0-135">请求</span><span class="sxs-lookup"><span data-stu-id="b43b0-135">Request</span></span>
<span data-ttu-id="b43b0-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b43b0-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="b43b0-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="b43b0-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_resetunseencount"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/resetUnseenCount
```
# <a name="c"></a>[<span data-ttu-id="b43b0-138">C#</span><span class="sxs-lookup"><span data-stu-id="b43b0-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-resetunseencount-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b43b0-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b43b0-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-resetunseencount-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b43b0-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b43b0-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-resetunseencount-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b43b0-141">Java</span><span class="sxs-lookup"><span data-stu-id="b43b0-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-resetunseencount-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b43b0-142">响应</span><span class="sxs-lookup"><span data-stu-id="b43b0-142">Response</span></span>
<span data-ttu-id="b43b0-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b43b0-143">The following is an example of the response.</span></span> 
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
  "description": "group: resetUnseenCount",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


