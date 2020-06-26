---
title: 组：subscribeByMail
description: 调用此方法可使当前用户在该组中收到有关该组的新帖子、事件和文件的电子邮件通知。
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: d5865086ff1fd97af8e9897cde66a5cdd1599923
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44895788"
---
# <a name="group-subscribebymail"></a><span data-ttu-id="f6c6c-103">组：subscribeByMail</span><span class="sxs-lookup"><span data-stu-id="f6c6c-103">group: subscribeByMail</span></span>

<span data-ttu-id="f6c6c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6c6c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6c6c-105">调用此方法可使当前用户在该组中收到有关该组的新帖子、事件和文件的电子邮件通知。</span><span class="sxs-lookup"><span data-stu-id="f6c6c-105">Calling this method will enable the current user to receive email notifications for this group, about new posts, events, and files in that group.</span></span> <span data-ttu-id="f6c6c-106">仅支持 Microsoft 365 组。</span><span class="sxs-lookup"><span data-stu-id="f6c6c-106">Supported for Microsoft 365 groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="f6c6c-107">权限</span><span class="sxs-lookup"><span data-stu-id="f6c6c-107">Permissions</span></span>
<span data-ttu-id="f6c6c-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="f6c6c-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="f6c6c-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f6c6c-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f6c6c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f6c6c-110">Permission type</span></span>      | <span data-ttu-id="f6c6c-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f6c6c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f6c6c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f6c6c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f6c6c-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6c6c-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f6c6c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f6c6c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f6c6c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f6c6c-115">Not supported.</span></span>    |
|<span data-ttu-id="f6c6c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f6c6c-116">Application</span></span> | <span data-ttu-id="f6c6c-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="f6c6c-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f6c6c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f6c6c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/subscribeByMail
```
## <a name="request-headers"></a><span data-ttu-id="f6c6c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f6c6c-119">Request headers</span></span>
| <span data-ttu-id="f6c6c-120">标头</span><span class="sxs-lookup"><span data-stu-id="f6c6c-120">Header</span></span>       | <span data-ttu-id="f6c6c-121">值</span><span class="sxs-lookup"><span data-stu-id="f6c6c-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f6c6c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6c6c-122">Authorization</span></span>  | <span data-ttu-id="f6c6c-123">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="f6c6c-123">Bearer {token}.</span></span> <span data-ttu-id="f6c6c-124">Required.</span><span class="sxs-lookup"><span data-stu-id="f6c6c-124">Required.</span></span>  |
| <span data-ttu-id="f6c6c-125">Prefer</span><span class="sxs-lookup"><span data-stu-id="f6c6c-125">Prefer</span></span> | <span data-ttu-id="f6c6c-126">return=minimal。</span><span class="sxs-lookup"><span data-stu-id="f6c6c-126">return=minimal.</span></span> <span data-ttu-id="f6c6c-127">如果 minimal 响应头包含在请求头中，那么成功响应返回 `204 No Content` 代码。</span><span class="sxs-lookup"><span data-stu-id="f6c6c-127">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="f6c6c-128">可选。</span><span class="sxs-lookup"><span data-stu-id="f6c6c-128">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="f6c6c-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="f6c6c-129">Request body</span></span>

## <a name="response"></a><span data-ttu-id="f6c6c-130">响应</span><span class="sxs-lookup"><span data-stu-id="f6c6c-130">Response</span></span>
<span data-ttu-id="f6c6c-131">If successful, this method returns `200 OK` response code.</span><span class="sxs-lookup"><span data-stu-id="f6c6c-131">If successful, this method returns `200 OK` response code.</span></span> <span data-ttu-id="f6c6c-132">It does not return anything in the response body.</span><span class="sxs-lookup"><span data-stu-id="f6c6c-132">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6c6c-133">示例</span><span class="sxs-lookup"><span data-stu-id="f6c6c-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="f6c6c-134">请求</span><span class="sxs-lookup"><span data-stu-id="f6c6c-134">Request</span></span>
<span data-ttu-id="f6c6c-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f6c6c-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f6c6c-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="f6c6c-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_subscribebymail"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/subscribeByMail
```
# <a name="c"></a>[<span data-ttu-id="f6c6c-137">C#</span><span class="sxs-lookup"><span data-stu-id="f6c6c-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-subscribebymail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f6c6c-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f6c6c-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-subscribebymail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f6c6c-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f6c6c-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-subscribebymail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f6c6c-140">响应</span><span class="sxs-lookup"><span data-stu-id="f6c6c-140">Response</span></span>
<span data-ttu-id="f6c6c-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f6c6c-141">The following is an example of the response.</span></span> 
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
  "description": "group: subscribeByMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
