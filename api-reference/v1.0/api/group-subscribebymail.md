---
title: 组：subscribeByMail
description: 调用此方法将允许当前用户接收有关该组中新帖子、活动和文件的电子邮件通知。仅支持 Office 365 组。
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 574e052cf93031cd1c868c43e837aa0e11e021ce
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/09/2020
ms.locfileid: "44178022"
---
# <a name="group-subscribebymail"></a><span data-ttu-id="21b62-104">组：subscribeByMail</span><span class="sxs-lookup"><span data-stu-id="21b62-104">group: subscribeByMail</span></span>

<span data-ttu-id="21b62-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="21b62-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="21b62-p102">调用此方法将允许当前用户接收有关该组中新帖子、活动和文件的电子邮件通知。仅支持 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="21b62-p102">Calling this method will enable the current user to receive email notifications for this group, about new posts, events, and files in that group. Supported for Office 365 groups only.</span></span>

## <a name="permissions"></a><span data-ttu-id="21b62-108">权限</span><span class="sxs-lookup"><span data-stu-id="21b62-108">Permissions</span></span>
<span data-ttu-id="21b62-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="21b62-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="21b62-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="21b62-111">Permission type</span></span>      | <span data-ttu-id="21b62-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="21b62-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="21b62-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="21b62-113">Delegated (work or school account)</span></span> | <span data-ttu-id="21b62-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="21b62-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="21b62-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="21b62-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="21b62-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="21b62-116">Not supported.</span></span>    |
|<span data-ttu-id="21b62-117">Application</span><span class="sxs-lookup"><span data-stu-id="21b62-117">Application</span></span> | <span data-ttu-id="21b62-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="21b62-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="21b62-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="21b62-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/subscribeByMail
```
## <a name="request-headers"></a><span data-ttu-id="21b62-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="21b62-120">Request headers</span></span>
| <span data-ttu-id="21b62-121">标头</span><span class="sxs-lookup"><span data-stu-id="21b62-121">Header</span></span>       | <span data-ttu-id="21b62-122">值</span><span class="sxs-lookup"><span data-stu-id="21b62-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="21b62-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="21b62-123">Authorization</span></span>  | <span data-ttu-id="21b62-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="21b62-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="21b62-126">Prefer</span><span class="sxs-lookup"><span data-stu-id="21b62-126">Prefer</span></span> | <span data-ttu-id="21b62-127">return=minimal。</span><span class="sxs-lookup"><span data-stu-id="21b62-127">return=minimal.</span></span> <span data-ttu-id="21b62-128">如果 minimal 响应头包含在请求头中，那么成功响应返回 `204 No Content` 代码。</span><span class="sxs-lookup"><span data-stu-id="21b62-128">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="21b62-129">可选。</span><span class="sxs-lookup"><span data-stu-id="21b62-129">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="21b62-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="21b62-130">Request body</span></span>
<span data-ttu-id="21b62-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="21b62-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="21b62-132">响应</span><span class="sxs-lookup"><span data-stu-id="21b62-132">Response</span></span>
<span data-ttu-id="21b62-p106">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="21b62-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="21b62-135">示例</span><span class="sxs-lookup"><span data-stu-id="21b62-135">Example</span></span>
#### <a name="request"></a><span data-ttu-id="21b62-136">请求</span><span class="sxs-lookup"><span data-stu-id="21b62-136">Request</span></span>
<span data-ttu-id="21b62-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="21b62-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="21b62-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="21b62-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_subscribebymail"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/subscribeByMail
```
# <a name="c"></a>[<span data-ttu-id="21b62-139">C#</span><span class="sxs-lookup"><span data-stu-id="21b62-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-subscribebymail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="21b62-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="21b62-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-subscribebymail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="21b62-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="21b62-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-subscribebymail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="21b62-142">Java</span><span class="sxs-lookup"><span data-stu-id="21b62-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-subscribebymail-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="21b62-143">响应</span><span class="sxs-lookup"><span data-stu-id="21b62-143">Response</span></span>
<span data-ttu-id="21b62-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="21b62-144">The following is an example of the response.</span></span> 
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
