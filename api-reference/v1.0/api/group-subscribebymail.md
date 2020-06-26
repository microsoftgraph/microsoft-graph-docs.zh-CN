---
title: 组：subscribeByMail
description: 调用此方法可使当前用户在该组中收到有关该组的新帖子、事件和文件的电子邮件通知。 仅支持 Microsoft 365 组。
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 8e3cb0d0a79da9ec246f0da50f17c3987695bb27
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897125"
---
# <a name="group-subscribebymail"></a><span data-ttu-id="cdc77-104">组：subscribeByMail</span><span class="sxs-lookup"><span data-stu-id="cdc77-104">group: subscribeByMail</span></span>

<span data-ttu-id="cdc77-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cdc77-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cdc77-106">调用此方法可使当前用户在该组中收到有关该组的新帖子、事件和文件的电子邮件通知。</span><span class="sxs-lookup"><span data-stu-id="cdc77-106">Calling this method will enable the current user to receive email notifications for this group, about new posts, events, and files in that group.</span></span> <span data-ttu-id="cdc77-107">仅支持 Microsoft 365 组。</span><span class="sxs-lookup"><span data-stu-id="cdc77-107">Supported for Microsoft 365 groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="cdc77-108">权限</span><span class="sxs-lookup"><span data-stu-id="cdc77-108">Permissions</span></span>
<span data-ttu-id="cdc77-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="cdc77-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="cdc77-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cdc77-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cdc77-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="cdc77-111">Permission type</span></span>      | <span data-ttu-id="cdc77-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cdc77-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cdc77-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cdc77-113">Delegated (work or school account)</span></span> | <span data-ttu-id="cdc77-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cdc77-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="cdc77-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cdc77-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cdc77-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="cdc77-116">Not supported.</span></span>    |
|<span data-ttu-id="cdc77-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="cdc77-117">Application</span></span> | <span data-ttu-id="cdc77-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="cdc77-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cdc77-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cdc77-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/subscribeByMail
```
## <a name="request-headers"></a><span data-ttu-id="cdc77-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="cdc77-120">Request headers</span></span>
| <span data-ttu-id="cdc77-121">标头</span><span class="sxs-lookup"><span data-stu-id="cdc77-121">Header</span></span>       | <span data-ttu-id="cdc77-122">值</span><span class="sxs-lookup"><span data-stu-id="cdc77-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cdc77-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cdc77-123">Authorization</span></span>  | <span data-ttu-id="cdc77-124">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="cdc77-124">Bearer {token}.</span></span> <span data-ttu-id="cdc77-125">Required.</span><span class="sxs-lookup"><span data-stu-id="cdc77-125">Required.</span></span>  |
| <span data-ttu-id="cdc77-126">Prefer</span><span class="sxs-lookup"><span data-stu-id="cdc77-126">Prefer</span></span> | <span data-ttu-id="cdc77-127">return=minimal。</span><span class="sxs-lookup"><span data-stu-id="cdc77-127">return=minimal.</span></span> <span data-ttu-id="cdc77-128">如果 minimal 响应头包含在请求头中，那么成功响应返回 `204 No Content` 代码。</span><span class="sxs-lookup"><span data-stu-id="cdc77-128">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="cdc77-129">可选。</span><span class="sxs-lookup"><span data-stu-id="cdc77-129">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="cdc77-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="cdc77-130">Request body</span></span>
<span data-ttu-id="cdc77-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cdc77-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cdc77-132">响应</span><span class="sxs-lookup"><span data-stu-id="cdc77-132">Response</span></span>
<span data-ttu-id="cdc77-133">If successful, this method returns `200 OK` response code.</span><span class="sxs-lookup"><span data-stu-id="cdc77-133">If successful, this method returns `200 OK` response code.</span></span> <span data-ttu-id="cdc77-134">It does not return anything in the response body.</span><span class="sxs-lookup"><span data-stu-id="cdc77-134">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cdc77-135">示例</span><span class="sxs-lookup"><span data-stu-id="cdc77-135">Example</span></span>
#### <a name="request"></a><span data-ttu-id="cdc77-136">请求</span><span class="sxs-lookup"><span data-stu-id="cdc77-136">Request</span></span>
<span data-ttu-id="cdc77-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="cdc77-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cdc77-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="cdc77-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_subscribebymail"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/subscribeByMail
```
# <a name="c"></a>[<span data-ttu-id="cdc77-139">C#</span><span class="sxs-lookup"><span data-stu-id="cdc77-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-subscribebymail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cdc77-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cdc77-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-subscribebymail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cdc77-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cdc77-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-subscribebymail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cdc77-142">Java</span><span class="sxs-lookup"><span data-stu-id="cdc77-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-subscribebymail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="cdc77-143">响应</span><span class="sxs-lookup"><span data-stu-id="cdc77-143">Response</span></span>
<span data-ttu-id="cdc77-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="cdc77-144">The following is an example of the response.</span></span> 
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
