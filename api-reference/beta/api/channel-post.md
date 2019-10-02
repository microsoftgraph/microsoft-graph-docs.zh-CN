---
title: 创建频道
description: 在 Microsoft 团队中创建请求正文中指定的新频道。
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 470e0da36be8cf1d68a55d723fee8f39c737ebac
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37355916"
---
# <a name="create-channel"></a><span data-ttu-id="a0932-103">创建频道</span><span class="sxs-lookup"><span data-stu-id="a0932-103">Create Channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0932-104">在 Microsoft 团队中创建请求正文中指定的新[频道](../resources/channel.md)。</span><span class="sxs-lookup"><span data-stu-id="a0932-104">Create a new [channel](../resources/channel.md) in a Microsoft Team, as specified in the request body.</span></span>

## <a name="permissions"></a><span data-ttu-id="a0932-105">权限</span><span class="sxs-lookup"><span data-stu-id="a0932-105">Permissions</span></span>

<span data-ttu-id="a0932-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a0932-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0932-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="a0932-108">Permission type</span></span>      | <span data-ttu-id="a0932-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a0932-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a0932-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a0932-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a0932-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0932-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="a0932-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a0932-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a0932-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="a0932-113">Not supported.</span></span>    |
|<span data-ttu-id="a0932-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="a0932-114">Application</span></span> | <span data-ttu-id="a0932-115">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0932-115">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="a0932-116">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="a0932-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="a0932-117">全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的团队。</span><span class="sxs-lookup"><span data-stu-id="a0932-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="a0932-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a0932-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels
```

## <a name="request-headers"></a><span data-ttu-id="a0932-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a0932-119">Request headers</span></span>

| <span data-ttu-id="a0932-120">标头</span><span class="sxs-lookup"><span data-stu-id="a0932-120">Header</span></span>       | <span data-ttu-id="a0932-121">值</span><span class="sxs-lookup"><span data-stu-id="a0932-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a0932-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a0932-122">Authorization</span></span>  | <span data-ttu-id="a0932-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a0932-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a0932-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a0932-125">Content-Type</span></span>  | <span data-ttu-id="a0932-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a0932-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a0932-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a0932-127">Request body</span></span>

<span data-ttu-id="a0932-128">在请求正文中，提供 [channel](../resources/channel.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a0932-128">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a0932-129">响应</span><span class="sxs-lookup"><span data-stu-id="a0932-129">Response</span></span>

<span data-ttu-id="a0932-130">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [channel](../resources/channel.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a0932-130">If successful, this method returns `201 Created` response code and [channel](../resources/channel.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a0932-131">示例</span><span class="sxs-lookup"><span data-stu-id="a0932-131">Examples</span></span>

### <a name="example-1-create-a-standard-channel"></a><span data-ttu-id="a0932-132">示例1：创建标准通道</span><span class="sxs-lookup"><span data-stu-id="a0932-132">Example 1: Create a standard channel</span></span>

#### <a name="request"></a><span data-ttu-id="a0932-133">请求</span><span class="sxs-lookup"><span data-stu-id="a0932-133">Request</span></span>

<span data-ttu-id="a0932-134">下面的示例展示了创建标准频道的请求。</span><span class="sxs-lookup"><span data-stu-id="a0932-134">The following example shows a request to create a standard channel.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a0932-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="a0932-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_channel_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels
Content-type: application/json

{
  "displayName": "Architecture Discussion",
  "description": "This channel is where we debate all future architecture plans",
  "membershipType": "standard"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a0932-136">C#</span><span class="sxs-lookup"><span data-stu-id="a0932-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-channel-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a0932-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a0932-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-channel-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a0932-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a0932-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-channel-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="a0932-139">响应</span><span class="sxs-lookup"><span data-stu-id="a0932-139">Response</span></span>

<span data-ttu-id="a0932-140">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="a0932-140">The following example shows the response.</span></span>

> <span data-ttu-id="a0932-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a0932-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
  "id": "id-value",
  "displayName": "Architecture Discussion",
  "description": "This channel is where we debate all future architecture plans"
}
```

### <a name="example-2-create-private-channel-on-behalf-of-user"></a><span data-ttu-id="a0932-143">示例2：代表用户创建专用通道</span><span class="sxs-lookup"><span data-stu-id="a0932-143">Example 2: Create private channel on behalf of user</span></span>

#### <a name="request"></a><span data-ttu-id="a0932-144">请求</span><span class="sxs-lookup"><span data-stu-id="a0932-144">Request</span></span>

<span data-ttu-id="a0932-145">下面的示例演示了创建专用通道并将用户添加为团队所有者的请求。</span><span class="sxs-lookup"><span data-stu-id="a0932-145">The following example shows a request to create a private channel and add a user as an team owner.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="a0932-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="a0932-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_channel_from_user"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{group_id}/channels
Content-type: application/json

{
  "@odata.type": "#Microsoft.Teams.Core.channel",
  "membershipType": "private",
  "displayName": "My First Private Channel",
  "description": "This is my first private channels",
  "members":
     [
        {
           "@odata.type":"#microsoft.graph.aadUserConversationMember",
           "user@odata.bind":"https://graph.microsoft.com/beta/users('{user_id}')",
           "roles":["owner"]
        }
     ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a0932-147">C#</span><span class="sxs-lookup"><span data-stu-id="a0932-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-channel-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a0932-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a0932-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-channel-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a0932-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a0932-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-channel-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a0932-150">响应</span><span class="sxs-lookup"><span data-stu-id="a0932-150">Response</span></span>

<span data-ttu-id="a0932-151">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="a0932-151">The following example shows the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('{group_id}')/channels/$entity",
    "id": "{channel_id}",
    "displayName": "My First Private Channel",
    "description": "This is my first private channels",
    "isFavoriteByDefault": null,
    "email": "",
    "webUrl": "https://teams.microsoft.com/l/channel/{channel_id}/My%20First%20Private%20Channel?groupId={group_id}&tenantId={tenant_id}",
    "membershipType": "private"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
