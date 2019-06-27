---
title: 创建 rejectedSender
description: 将新用户或组添加到 acceptedSender 列表中。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 10f8159712865bd41756f8efa298978548b23555
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35262893"
---
# <a name="create-rejectedsender"></a><span data-ttu-id="eeeb7-103">创建 rejectedSender</span><span class="sxs-lookup"><span data-stu-id="eeeb7-103">Create rejectedSender</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eeeb7-104">将新用户或组添加到 acceptedSender 列表中。</span><span class="sxs-lookup"><span data-stu-id="eeeb7-104">Add a new user or group to the rejectedSender list.</span></span>

<span data-ttu-id="eeeb7-p101">在请求主体的 `@odata.id` 中指定用户或组。已拒绝的发件人列表中的用户无法发布到组对话（在 POST 请求 URL 中标识）。确保未在拒绝的发件人和接受的发件人列表中指定同一用户或组，否则会发生错误。</span><span class="sxs-lookup"><span data-stu-id="eeeb7-p101">Specify the user or group in `@odata.id` in the request body. Users in the rejected senders list cannot post to conversations of the group (identified in the POST request URL). Make sure you do not specify the same user or group in the rejected senders and accepted senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="eeeb7-108">权限</span><span class="sxs-lookup"><span data-stu-id="eeeb7-108">Permissions</span></span>
<span data-ttu-id="eeeb7-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="eeeb7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eeeb7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="eeeb7-111">Permission type</span></span>      | <span data-ttu-id="eeeb7-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="eeeb7-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eeeb7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eeeb7-113">Delegated (work or school account)</span></span> | <span data-ttu-id="eeeb7-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eeeb7-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="eeeb7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eeeb7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eeeb7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="eeeb7-116">Not supported.</span></span>    |
|<span data-ttu-id="eeeb7-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="eeeb7-117">Application</span></span> | <span data-ttu-id="eeeb7-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="eeeb7-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="eeeb7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eeeb7-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/rejectedSenders/$ref
```

## <a name="request-headers"></a><span data-ttu-id="eeeb7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="eeeb7-120">Request headers</span></span>
| <span data-ttu-id="eeeb7-121">标头</span><span class="sxs-lookup"><span data-stu-id="eeeb7-121">Header</span></span>       | <span data-ttu-id="eeeb7-122">值</span><span class="sxs-lookup"><span data-stu-id="eeeb7-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="eeeb7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="eeeb7-123">Authorization</span></span>  | <span data-ttu-id="eeeb7-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="eeeb7-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="eeeb7-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="eeeb7-126">Request body</span></span>
<span data-ttu-id="eeeb7-127">在请求正文中，提供 user 或 group 对象的 ID。</span><span class="sxs-lookup"><span data-stu-id="eeeb7-127">In the request body, supply the id of a user or group object.</span></span>

## <a name="response"></a><span data-ttu-id="eeeb7-128">响应</span><span class="sxs-lookup"><span data-stu-id="eeeb7-128">Response</span></span>
<span data-ttu-id="eeeb7-129">此方法返回 `204 No Content` 响应代码，不返回任何响应正文。</span><span class="sxs-lookup"><span data-stu-id="eeeb7-129">This method returns `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="eeeb7-130">示例</span><span class="sxs-lookup"><span data-stu-id="eeeb7-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="eeeb7-131">请求</span><span class="sxs-lookup"><span data-stu-id="eeeb7-131">Request</span></span>
<span data-ttu-id="eeeb7-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="eeeb7-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_rejectedsender"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/rejectedSenders/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id":"https://graph.microsoft.com/beta/users/alexd@contoso.com"
}
```

#### <a name="response"></a><span data-ttu-id="eeeb7-133">响应</span><span class="sxs-lookup"><span data-stu-id="eeeb7-133">Response</span></span>
<span data-ttu-id="eeeb7-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="eeeb7-134">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="eeeb7-135">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="eeeb7-135">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="eeeb7-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="eeeb7-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_rejectedsender-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="eeeb7-137">目标-C</span><span class="sxs-lookup"><span data-stu-id="eeeb7-137">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_rejectedsender-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create rejectedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-post-rejectedsenders.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/group-post-rejectedsenders.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
