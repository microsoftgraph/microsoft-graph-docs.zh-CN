---
title: 删除 acceptedSender
description: 向 acceptedSender 列表中添加新用户或组。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 6f557cd1d4884f765334abe394610c520db68ead
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33329743"
---
# <a name="create-acceptedsender"></a><span data-ttu-id="89c94-103">删除 acceptedSender</span><span class="sxs-lookup"><span data-stu-id="89c94-103">Create acceptedSender</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="89c94-104">向 acceptedSender 列表中添加新用户或组。</span><span class="sxs-lookup"><span data-stu-id="89c94-104">Add a new user or group to the acceptedSender list.</span></span>

<span data-ttu-id="89c94-p101">在请求主体的 `@odata.id` 中指定用户或组。已接受的发件人列表中的用户可以发布到组对话。确保未在接受的发件人和拒绝的发件人列表中指定同一用户或组，否则会发生错误。</span><span class="sxs-lookup"><span data-stu-id="89c94-p101">Specify the user or group in `@odata.id` in the request body. Users in the accepted senders list can post to conversations of the group . Make sure you do not specify the same user or group in the accepted senders and rejected senders lists, otherwise you will get an error.</span></span>

## <a name="permissions"></a><span data-ttu-id="89c94-108">权限</span><span class="sxs-lookup"><span data-stu-id="89c94-108">Permissions</span></span>
<span data-ttu-id="89c94-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="89c94-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89c94-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="89c94-111">Permission type</span></span>      | <span data-ttu-id="89c94-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="89c94-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="89c94-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="89c94-113">Delegated (work or school account)</span></span> | <span data-ttu-id="89c94-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89c94-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="89c94-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="89c94-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89c94-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="89c94-116">Not supported.</span></span>    |
|<span data-ttu-id="89c94-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="89c94-117">Application</span></span> | <span data-ttu-id="89c94-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="89c94-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="89c94-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="89c94-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/acceptedSenders/$ref
```
## <a name="request-headers"></a><span data-ttu-id="89c94-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="89c94-120">Request headers</span></span>
| <span data-ttu-id="89c94-121">标头</span><span class="sxs-lookup"><span data-stu-id="89c94-121">Header</span></span>       | <span data-ttu-id="89c94-122">值</span><span class="sxs-lookup"><span data-stu-id="89c94-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="89c94-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="89c94-123">Authorization</span></span>  | <span data-ttu-id="89c94-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="89c94-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="89c94-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="89c94-126">Request body</span></span>
<span data-ttu-id="89c94-127">在请求正文中，提供 user 或 group 对象的 ID。</span><span class="sxs-lookup"><span data-stu-id="89c94-127">In the request body, supply the id of a user or group object.</span></span>

## <a name="response"></a><span data-ttu-id="89c94-128">响应</span><span class="sxs-lookup"><span data-stu-id="89c94-128">Response</span></span>
<span data-ttu-id="89c94-129">此方法返回 `204 No Content` 响应代码，不返回任何响应正文。</span><span class="sxs-lookup"><span data-stu-id="89c94-129">This method returns `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="89c94-130">示例</span><span class="sxs-lookup"><span data-stu-id="89c94-130">Example</span></span>
#### <a name="request"></a><span data-ttu-id="89c94-131">请求</span><span class="sxs-lookup"><span data-stu-id="89c94-131">Request</span></span>
<span data-ttu-id="89c94-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="89c94-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_acceptedsender"
}-->
```http
POST https://graph.microsoft.com/beta/groups/{id}/acceptedSenders/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id":"https://graph.microsoft.com/beta/users/alexd@contoso.com"
}
```

#### <a name="response"></a><span data-ttu-id="89c94-133">响应</span><span class="sxs-lookup"><span data-stu-id="89c94-133">Response</span></span>
<span data-ttu-id="89c94-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="89c94-134">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create acceptedSender",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
