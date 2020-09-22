---
title: 组：unsubscribeByMail
description: 调用此方法将禁用当前用户接收此组的电子邮件通知。此组中的新帖子、事件和文件。
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 017b834908c08adc136837fd0af07cb0a3e59f53
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48001979"
---
# <a name="group-unsubscribebymail"></a><span data-ttu-id="555ec-103">组：unsubscribeByMail</span><span class="sxs-lookup"><span data-stu-id="555ec-103">group: unsubscribeByMail</span></span>

<span data-ttu-id="555ec-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="555ec-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="555ec-105">调用此方法将禁用当前用户接收此组的电子邮件通知。此组中的新帖子、事件和文件。</span><span class="sxs-lookup"><span data-stu-id="555ec-105">Calling this method will disable the current user to receive email notifications for this group about new posts, events, and files in that group.</span></span> <span data-ttu-id="555ec-106">仅支持 Microsoft 365 组。</span><span class="sxs-lookup"><span data-stu-id="555ec-106">Supported for Microsoft 365 groups only.</span></span> 

## <a name="permissions"></a><span data-ttu-id="555ec-107">权限</span><span class="sxs-lookup"><span data-stu-id="555ec-107">Permissions</span></span>
<span data-ttu-id="555ec-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="555ec-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="555ec-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="555ec-110">Permission type</span></span>      | <span data-ttu-id="555ec-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="555ec-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="555ec-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="555ec-112">Delegated (work or school account)</span></span> | <span data-ttu-id="555ec-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="555ec-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="555ec-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="555ec-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="555ec-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="555ec-115">Not supported.</span></span>    |
|<span data-ttu-id="555ec-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="555ec-116">Application</span></span> | <span data-ttu-id="555ec-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="555ec-117">Group.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="555ec-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="555ec-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/unsubscribeByMail
```

## <a name="request-headers"></a><span data-ttu-id="555ec-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="555ec-119">Request headers</span></span>
| <span data-ttu-id="555ec-120">标头</span><span class="sxs-lookup"><span data-stu-id="555ec-120">Header</span></span>       | <span data-ttu-id="555ec-121">值</span><span class="sxs-lookup"><span data-stu-id="555ec-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="555ec-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="555ec-122">Authorization</span></span>  | <span data-ttu-id="555ec-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="555ec-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="555ec-125">Prefer</span><span class="sxs-lookup"><span data-stu-id="555ec-125">Prefer</span></span> | <span data-ttu-id="555ec-126">return=minimal。</span><span class="sxs-lookup"><span data-stu-id="555ec-126">return=minimal.</span></span> <span data-ttu-id="555ec-127">如果 minimal 响应头包含在请求头中，那么成功响应返回 `204 No Content` 代码。</span><span class="sxs-lookup"><span data-stu-id="555ec-127">If minimal response header is included in the request header, then a successful response returns `204 No Content` code.</span></span> <span data-ttu-id="555ec-128">可选。</span><span class="sxs-lookup"><span data-stu-id="555ec-128">Optional.</span></span>  | 

## <a name="request-body"></a><span data-ttu-id="555ec-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="555ec-129">Request body</span></span>
 <span data-ttu-id="555ec-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="555ec-130">Do not supply a request body for this method.</span></span> 

## <a name="response"></a><span data-ttu-id="555ec-131">响应</span><span class="sxs-lookup"><span data-stu-id="555ec-131">Response</span></span>
<span data-ttu-id="555ec-p105">如果成功，此方法返回 `200 OK` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="555ec-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="555ec-134">示例</span><span class="sxs-lookup"><span data-stu-id="555ec-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="555ec-135">请求</span><span class="sxs-lookup"><span data-stu-id="555ec-135">Request</span></span>
<span data-ttu-id="555ec-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="555ec-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="555ec-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="555ec-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_unsubscribebymail"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/unsubscribeByMail
```
# <a name="c"></a>[<span data-ttu-id="555ec-138">C#</span><span class="sxs-lookup"><span data-stu-id="555ec-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-unsubscribebymail-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="555ec-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="555ec-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-unsubscribebymail-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="555ec-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="555ec-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-unsubscribebymail-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="555ec-141">响应</span><span class="sxs-lookup"><span data-stu-id="555ec-141">Response</span></span>
<span data-ttu-id="555ec-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="555ec-142">The following is an example of the response.</span></span> 
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


