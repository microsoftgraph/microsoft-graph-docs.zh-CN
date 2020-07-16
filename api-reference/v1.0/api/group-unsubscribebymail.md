---
title: 组：unsubscribeByMail
description: '调用此方法可使当前用户在该组中收到有关该组的新帖子、事件和文件的电子邮件通知。 仅支持 Microsoft 365 组。 '
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: afbee22fc9c51cd9b7428b89677907efc3786c1c
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897118"
---
# <a name="group-unsubscribebymail"></a><span data-ttu-id="f34c4-104">组：unsubscribeByMail</span><span class="sxs-lookup"><span data-stu-id="f34c4-104">group: unsubscribeByMail</span></span>

<span data-ttu-id="f34c4-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f34c4-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f34c4-106">调用此方法可使当前用户在该组中收到有关该组的新帖子、事件和文件的电子邮件通知。</span><span class="sxs-lookup"><span data-stu-id="f34c4-106">Calling this method will prevent the current user from receiving email notifications for this group about new posts, events, and files in that group.</span></span> <span data-ttu-id="f34c4-107">仅支持 Microsoft 365 组。</span><span class="sxs-lookup"><span data-stu-id="f34c4-107">Supported for Microsoft 365 groups only.</span></span> 

## <a name="permissions"></a><span data-ttu-id="f34c4-108">权限</span><span class="sxs-lookup"><span data-stu-id="f34c4-108">Permissions</span></span>
<span data-ttu-id="f34c4-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f34c4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f34c4-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f34c4-111">Permission type</span></span>      | <span data-ttu-id="f34c4-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f34c4-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f34c4-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f34c4-113">Delegated (work or school account)</span></span> | <span data-ttu-id="f34c4-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f34c4-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f34c4-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f34c4-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f34c4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f34c4-116">Not supported.</span></span>    |
|<span data-ttu-id="f34c4-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f34c4-117">Application</span></span> | <span data-ttu-id="f34c4-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="f34c4-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f34c4-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f34c4-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/unsubscribeByMail
```
## <a name="request-headers"></a><span data-ttu-id="f34c4-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f34c4-120">Request headers</span></span>
| <span data-ttu-id="f34c4-121">标头</span><span class="sxs-lookup"><span data-stu-id="f34c4-121">Header</span></span>       | <span data-ttu-id="f34c4-122">值</span><span class="sxs-lookup"><span data-stu-id="f34c4-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f34c4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f34c4-123">Authorization</span></span>  | <span data-ttu-id="f34c4-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f34c4-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f34c4-126">Prefer</span><span class="sxs-lookup"><span data-stu-id="f34c4-126">Prefer</span></span> | <span data-ttu-id="f34c4-127">return=minimal。</span><span class="sxs-lookup"><span data-stu-id="f34c4-127">return=minimal.</span></span> <span data-ttu-id="f34c4-128">如果 minimal 响应头包含在请求头中，那么成功响应返回 `204 No Content` 代码。</span><span class="sxs-lookup"><span data-stu-id="f34c4-128">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="f34c4-129">可选。</span><span class="sxs-lookup"><span data-stu-id="f34c4-129">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="f34c4-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="f34c4-130">Request body</span></span>
<span data-ttu-id="f34c4-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f34c4-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f34c4-132">响应</span><span class="sxs-lookup"><span data-stu-id="f34c4-132">Response</span></span>
<span data-ttu-id="f34c4-p106">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="f34c4-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f34c4-135">示例</span><span class="sxs-lookup"><span data-stu-id="f34c4-135">Example</span></span>
#### <a name="request"></a><span data-ttu-id="f34c4-136">请求</span><span class="sxs-lookup"><span data-stu-id="f34c4-136">Request</span></span>
<span data-ttu-id="f34c4-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f34c4-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f34c4-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="f34c4-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_unsubscribebymail"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/unsubscribeByMail
```
# <a name="c"></a>[<span data-ttu-id="f34c4-139">C#</span><span class="sxs-lookup"><span data-stu-id="f34c4-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-unsubscribebymail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f34c4-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f34c4-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-unsubscribebymail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f34c4-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f34c4-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-unsubscribebymail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f34c4-142">Java</span><span class="sxs-lookup"><span data-stu-id="f34c4-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-unsubscribebymail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f34c4-143">响应</span><span class="sxs-lookup"><span data-stu-id="f34c4-143">Response</span></span>
<span data-ttu-id="f34c4-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f34c4-144">The following is an example of the response.</span></span> 
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
  "description": "group: unsubscribeByMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
