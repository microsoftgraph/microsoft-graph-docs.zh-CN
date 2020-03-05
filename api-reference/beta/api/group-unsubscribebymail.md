---
title: 组：unsubscribeByMail
description: '调用此方法将禁用当前用户接收此组的电子邮件通知。此组中的新帖子、事件和文件。 仅支持 Office 365 组。 '
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 252fd8fbcc878c7d77818e2215cd8a06ea4722b0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42418229"
---
# <a name="group-unsubscribebymail"></a><span data-ttu-id="bd310-104">组：unsubscribeByMail</span><span class="sxs-lookup"><span data-stu-id="bd310-104">group: unsubscribeByMail</span></span>

<span data-ttu-id="bd310-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="bd310-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd310-106">调用此方法将禁用当前用户接收此组的电子邮件通知。此组中的新帖子、事件和文件。</span><span class="sxs-lookup"><span data-stu-id="bd310-106">Calling this method will disable the current user to receive email notifications for this group about new posts, events, and files in that group.</span></span> <span data-ttu-id="bd310-107">仅支持 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="bd310-107">Supported for Office 365 groups only.</span></span> 

## <a name="permissions"></a><span data-ttu-id="bd310-108">权限</span><span class="sxs-lookup"><span data-stu-id="bd310-108">Permissions</span></span>
<span data-ttu-id="bd310-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bd310-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd310-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="bd310-111">Permission type</span></span>      | <span data-ttu-id="bd310-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bd310-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bd310-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bd310-113">Delegated (work or school account)</span></span> | <span data-ttu-id="bd310-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd310-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="bd310-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bd310-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd310-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bd310-116">Not supported.</span></span>    |
|<span data-ttu-id="bd310-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="bd310-117">Application</span></span> | <span data-ttu-id="bd310-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd310-118">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bd310-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bd310-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/unsubscribeByMail
```

## <a name="request-headers"></a><span data-ttu-id="bd310-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="bd310-120">Request headers</span></span>
| <span data-ttu-id="bd310-121">标头</span><span class="sxs-lookup"><span data-stu-id="bd310-121">Header</span></span>       | <span data-ttu-id="bd310-122">值</span><span class="sxs-lookup"><span data-stu-id="bd310-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bd310-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bd310-123">Authorization</span></span>  | <span data-ttu-id="bd310-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bd310-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="bd310-126">Prefer</span><span class="sxs-lookup"><span data-stu-id="bd310-126">Prefer</span></span> | <span data-ttu-id="bd310-127">return=minimal。</span><span class="sxs-lookup"><span data-stu-id="bd310-127">return=minimal.</span></span> <span data-ttu-id="bd310-128">如果 minimal 响应头包含在请求头中，那么成功响应返回 `204 No Content` 代码。</span><span class="sxs-lookup"><span data-stu-id="bd310-128">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="bd310-129">可选。</span><span class="sxs-lookup"><span data-stu-id="bd310-129">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="bd310-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="bd310-130">Request body</span></span>
 <span data-ttu-id="bd310-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bd310-131">Do not supply a request body for this method.</span></span> 

## <a name="response"></a><span data-ttu-id="bd310-132">响应</span><span class="sxs-lookup"><span data-stu-id="bd310-132">Response</span></span>
<span data-ttu-id="bd310-p106">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="bd310-p106">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd310-135">示例</span><span class="sxs-lookup"><span data-stu-id="bd310-135">Example</span></span>
#### <a name="request"></a><span data-ttu-id="bd310-136">请求</span><span class="sxs-lookup"><span data-stu-id="bd310-136">Request</span></span>
<span data-ttu-id="bd310-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bd310-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bd310-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="bd310-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_unsubscribebymail"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/unsubscribeByMail
```
# <a name="c"></a>[<span data-ttu-id="bd310-139">C#</span><span class="sxs-lookup"><span data-stu-id="bd310-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-unsubscribebymail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bd310-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bd310-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-unsubscribebymail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bd310-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bd310-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-unsubscribebymail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="bd310-142">响应</span><span class="sxs-lookup"><span data-stu-id="bd310-142">Response</span></span>
<span data-ttu-id="bd310-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="bd310-143">The following is an example of the response.</span></span> 
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
  "description": "group: unsubscribeByMail",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
