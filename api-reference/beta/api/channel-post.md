---
title: 创建频道
description: 在请求正文中指定的 Microsoft 团队中创建新通道。
localization_priority: Normal
author: laujan
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 41d0e74ef3e08102a5fb670159d0f7e51085817d
ms.sourcegitcommit: 60ced1be6ed8dd2d23263090a1cfbc16689bb043
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/28/2020
ms.locfileid: "48782822"
---
# <a name="create-channel"></a><span data-ttu-id="f7c3f-103">创建频道</span><span class="sxs-lookup"><span data-stu-id="f7c3f-103">Create channel</span></span>

<span data-ttu-id="f7c3f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7c3f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7c3f-105">在团队中创建一个新的 [频道](../resources/channel.md) ，如请求正文中所指定。</span><span class="sxs-lookup"><span data-stu-id="f7c3f-105">Create a new [channel](../resources/channel.md) in a team, as specified in the request body.</span></span>

## <a name="permissions"></a><span data-ttu-id="f7c3f-106">权限</span><span class="sxs-lookup"><span data-stu-id="f7c3f-106">Permissions</span></span>

<span data-ttu-id="f7c3f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f7c3f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7c3f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f7c3f-109">Permission type</span></span>      | <span data-ttu-id="f7c3f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f7c3f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7c3f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f7c3f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f7c3f-112">"创建"、"组"、"全部"、"全部"、"全部"</span><span class="sxs-lookup"><span data-stu-id="f7c3f-112">Channel.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="f7c3f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f7c3f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7c3f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f7c3f-114">Not supported.</span></span>    |
|<span data-ttu-id="f7c3f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f7c3f-115">Application</span></span> | <span data-ttu-id="f7c3f-116">例如，Group \*、信道. 创建、组读写全部、全部、团队合作。全部迁移</span><span class="sxs-lookup"><span data-stu-id="f7c3f-116">Channel.Create.Group\*, Channel.Create, Group.ReadWrite.All, Directory.ReadWrite.All, Teamwork.Migrate.All</span></span>|

> <span data-ttu-id="f7c3f-117">**注意** ：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="f7c3f-117">**Note** : Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="f7c3f-118">**注意** ：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="f7c3f-118">**Note** : This API supports admin permissions.</span></span> <span data-ttu-id="f7c3f-119">全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的团队。</span><span class="sxs-lookup"><span data-stu-id="f7c3f-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="f7c3f-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f7c3f-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels
```

## <a name="request-headers"></a><span data-ttu-id="f7c3f-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="f7c3f-121">Request headers</span></span>

| <span data-ttu-id="f7c3f-122">标头</span><span class="sxs-lookup"><span data-stu-id="f7c3f-122">Header</span></span>       | <span data-ttu-id="f7c3f-123">值</span><span class="sxs-lookup"><span data-stu-id="f7c3f-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f7c3f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7c3f-124">Authorization</span></span>  | <span data-ttu-id="f7c3f-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f7c3f-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f7c3f-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f7c3f-127">Content-Type</span></span>  | <span data-ttu-id="f7c3f-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="f7c3f-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f7c3f-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="f7c3f-130">Request body</span></span>

<span data-ttu-id="f7c3f-131">在请求正文中，提供 [channel](../resources/channel.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f7c3f-131">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f7c3f-132">响应</span><span class="sxs-lookup"><span data-stu-id="f7c3f-132">Response</span></span>

<span data-ttu-id="f7c3f-133">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [channel](../resources/channel.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f7c3f-133">If successful, this method returns a `201 Created` response code and a [channel](../resources/channel.md) object in the response body.</span></span>

<span data-ttu-id="f7c3f-134">如果请求不成功，此方法将返回 `400 Bad Request` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="f7c3f-134">If the request is unsuccessful, this method returns a `400 Bad Request` response code.</span></span> <span data-ttu-id="f7c3f-135">以下是此响应的常见原因：</span><span class="sxs-lookup"><span data-stu-id="f7c3f-135">The following are common reasons for this response:</span></span>

* <span data-ttu-id="f7c3f-136">**createdDateTime** 是在将来设置的。</span><span class="sxs-lookup"><span data-stu-id="f7c3f-136">**createdDateTime** is set in the future.</span></span>
* <span data-ttu-id="f7c3f-137">正确指定了 **createdDateTime** ，但 **channelCreationMode** 实例属性缺失或被设置为无效值。</span><span class="sxs-lookup"><span data-stu-id="f7c3f-137">**createdDateTime** is correctly specified but the **channelCreationMode** instance attribute is missing or set to an invalid value.</span></span>

## <a name="examples"></a><span data-ttu-id="f7c3f-138">示例</span><span class="sxs-lookup"><span data-stu-id="f7c3f-138">Examples</span></span>

### <a name="example-1-create-a-standard-channel"></a><span data-ttu-id="f7c3f-139">示例1：创建标准通道</span><span class="sxs-lookup"><span data-stu-id="f7c3f-139">Example 1: Create a standard channel</span></span>

#### <a name="request"></a><span data-ttu-id="f7c3f-140">请求</span><span class="sxs-lookup"><span data-stu-id="f7c3f-140">Request</span></span>

<span data-ttu-id="f7c3f-141">下面的示例展示了创建标准频道的请求。</span><span class="sxs-lookup"><span data-stu-id="f7c3f-141">The following example shows a request to create a standard channel.</span></span>

# <a name="http"></a>[<span data-ttu-id="f7c3f-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="f7c3f-142">HTTP</span></span>](#tab/http)
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

# <a name="c"></a>[<span data-ttu-id="f7c3f-143">C#</span><span class="sxs-lookup"><span data-stu-id="f7c3f-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-channel-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f7c3f-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f7c3f-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-channel-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f7c3f-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f7c3f-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-channel-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="f7c3f-146">响应</span><span class="sxs-lookup"><span data-stu-id="f7c3f-146">Response</span></span>

<span data-ttu-id="f7c3f-147">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="f7c3f-147">The following example shows the response.</span></span>

> <span data-ttu-id="f7c3f-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f7c3f-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-create-private-channel-on-behalf-of-user"></a><span data-ttu-id="f7c3f-150">示例2：代表用户创建专用通道</span><span class="sxs-lookup"><span data-stu-id="f7c3f-150">Example 2: Create private channel on behalf of user</span></span>

#### <a name="request"></a><span data-ttu-id="f7c3f-151">请求</span><span class="sxs-lookup"><span data-stu-id="f7c3f-151">Request</span></span>

<span data-ttu-id="f7c3f-152">下面的示例演示了创建专用通道并将用户添加为团队所有者的请求。</span><span class="sxs-lookup"><span data-stu-id="f7c3f-152">The following example shows a request to create a private channel and add a user as an team owner.</span></span>

# <a name="http"></a>[<span data-ttu-id="f7c3f-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="f7c3f-153">HTTP</span></span>](#tab/http)
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

# <a name="c"></a>[<span data-ttu-id="f7c3f-154">C#</span><span class="sxs-lookup"><span data-stu-id="f7c3f-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-channel-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f7c3f-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f7c3f-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-channel-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f7c3f-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f7c3f-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-channel-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<!-- markdownlint-disable MD001 -->
<!-- markdownlint-disable MD024 -->
#### <a name="response"></a><span data-ttu-id="f7c3f-157">响应</span><span class="sxs-lookup"><span data-stu-id="f7c3f-157">Response</span></span>

<span data-ttu-id="f7c3f-158">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="f7c3f-158">The following example shows the response.</span></span>

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

### <a name="example-3-create-a-channel-in-migration-mode"></a><span data-ttu-id="f7c3f-159">示例3：在迁移模式下创建通道</span><span class="sxs-lookup"><span data-stu-id="f7c3f-159">Example 3: Create a channel in migration mode</span></span>

#### <a name="request"></a><span data-ttu-id="f7c3f-160">请求</span><span class="sxs-lookup"><span data-stu-id="f7c3f-160">Request</span></span>

<span data-ttu-id="f7c3f-161">下面的示例演示如何为导入的邮件创建通道。</span><span class="sxs-lookup"><span data-stu-id="f7c3f-161">The following example shows how to create a channel for imported messages.</span></span>

```http
POST https://graph.microsoft.com/beta/teams/{id}/channels
Content-Type: application/json

{
  "@microsoft.graph.channelCreationMode": "migration",
  "displayName": "Architecture Discussion",
  "description": "This channel is where we debate all future architecture plans",
  "membershipType": "standard",
  "createdDateTime": "2020-03-14T11:22:17.067Z"
}
```

#### <a name="response"></a><span data-ttu-id="f7c3f-162">响应</span><span class="sxs-lookup"><span data-stu-id="f7c3f-162">Response</span></span>

```http
HTTP/1.1 202 Accepted
Location: /teams/{teamId}/channels/{channelId}/operations/{operationId}
Content-Location: /teams/{teamId}/channels/{channelId}
```

## <a name="see-also"></a><span data-ttu-id="f7c3f-163">另请参阅</span><span class="sxs-lookup"><span data-stu-id="f7c3f-163">See also</span></span>

* [<span data-ttu-id="f7c3f-164">完成频道迁移</span><span class="sxs-lookup"><span data-stu-id="f7c3f-164">Complete migration for a channel</span></span>](channel-completemigration.md)
* [<span data-ttu-id="f7c3f-165">使用 Microsoft Graph 将第三方平台消息导入 Teams</span><span class="sxs-lookup"><span data-stu-id="f7c3f-165">Import third-party platform messages to Teams using Microsoft Graph</span></span>](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams)
* [<span data-ttu-id="f7c3f-166">创建团队</span><span class="sxs-lookup"><span data-stu-id="f7c3f-166">Create team</span></span>](team-post.md)

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
