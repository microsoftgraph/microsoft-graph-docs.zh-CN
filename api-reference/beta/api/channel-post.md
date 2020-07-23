---
title: 创建频道
description: 在 Microsoft 团队中创建请求正文中指定的新频道。
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: d496f69b20613c4c42c7ce842d23299d653c2ada
ms.sourcegitcommit: fec7d5002dbeb8d58587c89f1b678d4a54645422
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/23/2020
ms.locfileid: "45384344"
---
# <a name="create-channel"></a><span data-ttu-id="78cd0-103">创建频道</span><span class="sxs-lookup"><span data-stu-id="78cd0-103">Create Channel</span></span>

<span data-ttu-id="78cd0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78cd0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78cd0-105">在 Microsoft 团队中创建请求正文中指定的新[频道](../resources/channel.md)。</span><span class="sxs-lookup"><span data-stu-id="78cd0-105">Create a new [channel](../resources/channel.md) in a Microsoft Team, as specified in the request body.</span></span>

## <a name="permissions"></a><span data-ttu-id="78cd0-106">权限</span><span class="sxs-lookup"><span data-stu-id="78cd0-106">Permissions</span></span>

<span data-ttu-id="78cd0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="78cd0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78cd0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="78cd0-109">Permission type</span></span>      | <span data-ttu-id="78cd0-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="78cd0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="78cd0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="78cd0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="78cd0-112">"创建"、"组"、"全部"、"全部"、"全部"</span><span class="sxs-lookup"><span data-stu-id="78cd0-112">Channel.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="78cd0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="78cd0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="78cd0-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="78cd0-114">Not supported.</span></span>    |
|<span data-ttu-id="78cd0-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="78cd0-115">Application</span></span> | <span data-ttu-id="78cd0-116">例如，Group \*、信道. Create、Group. All、</span><span class="sxs-lookup"><span data-stu-id="78cd0-116">Channel.Create.Group\*, Channel.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span></span>    |

> <span data-ttu-id="78cd0-117">**注意**：标记为 \* 的权限使用[特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="78cd0-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="78cd0-118">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="78cd0-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="78cd0-119">全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的团队。</span><span class="sxs-lookup"><span data-stu-id="78cd0-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="78cd0-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="78cd0-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels
```

## <a name="request-headers"></a><span data-ttu-id="78cd0-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="78cd0-121">Request headers</span></span>

| <span data-ttu-id="78cd0-122">标头</span><span class="sxs-lookup"><span data-stu-id="78cd0-122">Header</span></span>       | <span data-ttu-id="78cd0-123">值</span><span class="sxs-lookup"><span data-stu-id="78cd0-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="78cd0-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="78cd0-124">Authorization</span></span>  | <span data-ttu-id="78cd0-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="78cd0-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="78cd0-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="78cd0-127">Content-Type</span></span>  | <span data-ttu-id="78cd0-128">application/json</span><span class="sxs-lookup"><span data-stu-id="78cd0-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="78cd0-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="78cd0-129">Request body</span></span>

<span data-ttu-id="78cd0-130">在请求正文中，提供 [channel](../resources/channel.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="78cd0-130">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="78cd0-131">响应</span><span class="sxs-lookup"><span data-stu-id="78cd0-131">Response</span></span>

<span data-ttu-id="78cd0-132">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [channel](../resources/channel.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="78cd0-132">If successful, this method returns `201 Created` response code and [channel](../resources/channel.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="78cd0-133">示例</span><span class="sxs-lookup"><span data-stu-id="78cd0-133">Examples</span></span>

### <a name="example-1-create-a-standard-channel"></a><span data-ttu-id="78cd0-134">示例1：创建标准通道</span><span class="sxs-lookup"><span data-stu-id="78cd0-134">Example 1: Create a standard channel</span></span>

#### <a name="request"></a><span data-ttu-id="78cd0-135">请求</span><span class="sxs-lookup"><span data-stu-id="78cd0-135">Request</span></span>

<span data-ttu-id="78cd0-136">下面的示例展示了创建标准频道的请求。</span><span class="sxs-lookup"><span data-stu-id="78cd0-136">The following example shows a request to create a standard channel.</span></span>

# <a name="http"></a>[<span data-ttu-id="78cd0-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="78cd0-137">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="78cd0-138">C#</span><span class="sxs-lookup"><span data-stu-id="78cd0-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-channel-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="78cd0-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="78cd0-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-channel-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="78cd0-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="78cd0-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-channel-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="78cd0-141">响应</span><span class="sxs-lookup"><span data-stu-id="78cd0-141">Response</span></span>

<span data-ttu-id="78cd0-142">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="78cd0-142">The following example shows the response.</span></span>

> <span data-ttu-id="78cd0-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="78cd0-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 201

{
  "id": "id-value",
  "displayName": "Architecture Discussion",
  "description": "This channel is where we debate all future architecture plans"
}
```

### <a name="example-2-create-private-channel-on-behalf-of-user"></a><span data-ttu-id="78cd0-145">示例2：代表用户创建专用通道</span><span class="sxs-lookup"><span data-stu-id="78cd0-145">Example 2: Create private channel on behalf of user</span></span>

#### <a name="request"></a><span data-ttu-id="78cd0-146">请求</span><span class="sxs-lookup"><span data-stu-id="78cd0-146">Request</span></span>

<span data-ttu-id="78cd0-147">下面的示例演示了创建专用通道并将用户添加为团队所有者的请求。</span><span class="sxs-lookup"><span data-stu-id="78cd0-147">The following example shows a request to create a private channel and add a user as an team owner.</span></span>


# <a name="http"></a>[<span data-ttu-id="78cd0-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="78cd0-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_channel_from_user"
}-->

```http
POST https://graph.microsoft.com/beta/teams/{group_id}/channels
Content-type: application/json

{
  "@odata.type": "#Microsoft.Graph.channel",
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
# <a name="c"></a>[<span data-ttu-id="78cd0-149">C#</span><span class="sxs-lookup"><span data-stu-id="78cd0-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-channel-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="78cd0-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="78cd0-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-channel-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="78cd0-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="78cd0-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-channel-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="78cd0-152">响应</span><span class="sxs-lookup"><span data-stu-id="78cd0-152">Response</span></span>

<span data-ttu-id="78cd0-153">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="78cd0-153">The following example shows the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
} -->

```http
HTTP/1.1 201 Created
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
