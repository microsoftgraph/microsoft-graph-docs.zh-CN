---
title: 创建频道
description: 在团队中创建新频道，如请求正文中指定。
localization_priority: Normal
author: akjo
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: cca7ba2cfd6f69c6bbfda080c94c31013018657e
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/22/2021
ms.locfileid: "53059922"
---
# <a name="create-channel"></a><span data-ttu-id="d05eb-103">创建频道</span><span class="sxs-lookup"><span data-stu-id="d05eb-103">Create channel</span></span>

<span data-ttu-id="d05eb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d05eb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d05eb-105">在团队 [中创建新](../resources/channel.md) 频道，如请求正文中指定。</span><span class="sxs-lookup"><span data-stu-id="d05eb-105">Create a new [channel](../resources/channel.md) in a team, as specified in the request body.</span></span>

## <a name="permissions"></a><span data-ttu-id="d05eb-106">权限</span><span class="sxs-lookup"><span data-stu-id="d05eb-106">Permissions</span></span>

<span data-ttu-id="d05eb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d05eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d05eb-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d05eb-109">Permission type</span></span>      | <span data-ttu-id="d05eb-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d05eb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d05eb-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d05eb-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d05eb-112">Channel.Create、Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d05eb-112">Channel.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="d05eb-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d05eb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d05eb-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d05eb-114">Not supported.</span></span>    |
|<span data-ttu-id="d05eb-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d05eb-115">Application</span></span> | <span data-ttu-id="d05eb-116">Channel.Create.Group\*、Channel.Create、Teamwork.Migrate.All、Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d05eb-116">Channel.Create.Group\*, Channel.Create, Teamwork.Migrate.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="d05eb-117">**注意**：标有 \* 的权限用于 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="d05eb-117">**Note**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="d05eb-p102">**注意**：此 API 支持管理员权限。全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的团队。</span><span class="sxs-lookup"><span data-stu-id="d05eb-p102">**Note**: This API supports admin permissions. Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

> <span data-ttu-id="d05eb-120">**注意**：将来，Microsoft 可能会要求你或你的客户根据使用团队合作导入的数据量支付额外的费用。Migrate.All 和/或 [迁移 API。](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams)</span><span class="sxs-lookup"><span data-stu-id="d05eb-120">**Note**: In the future, Microsoft may require you or your customers to pay additional fees based on the amount of data imported using Teamwork.Migrate.All and/or [migration APIs](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams).</span></span>

## <a name="http-request"></a><span data-ttu-id="d05eb-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d05eb-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{team-id}/channels
```

## <a name="request-headers"></a><span data-ttu-id="d05eb-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="d05eb-122">Request headers</span></span>

| <span data-ttu-id="d05eb-123">标头</span><span class="sxs-lookup"><span data-stu-id="d05eb-123">Header</span></span>       | <span data-ttu-id="d05eb-124">值</span><span class="sxs-lookup"><span data-stu-id="d05eb-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="d05eb-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="d05eb-125">Authorization</span></span>  | <span data-ttu-id="d05eb-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d05eb-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="d05eb-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d05eb-128">Content-Type</span></span>  | <span data-ttu-id="d05eb-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="d05eb-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d05eb-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="d05eb-131">Request body</span></span>

<span data-ttu-id="d05eb-132">在请求正文中，提供 channel 对象的 JSON [表示](../resources/channel.md) 形式。</span><span class="sxs-lookup"><span data-stu-id="d05eb-132">In the request body, supply a JSON representation of a [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="d05eb-133">响应</span><span class="sxs-lookup"><span data-stu-id="d05eb-133">Response</span></span>

<span data-ttu-id="d05eb-134">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [channel](../resources/channel.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d05eb-134">If successful, this method returns a `201 Created` response code and a [channel](../resources/channel.md) object in the response body.</span></span>

<span data-ttu-id="d05eb-135">如果该请求成功，此方法返回 `400 Bad Request` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="d05eb-135">If the request is unsuccessful, this method returns a `400 Bad Request` response code.</span></span> <span data-ttu-id="d05eb-136">下面是出现此响应的常见原因：</span><span class="sxs-lookup"><span data-stu-id="d05eb-136">The following are common reasons for this response:</span></span>

* <span data-ttu-id="d05eb-137">**createdDateTime** 将在未来设置。</span><span class="sxs-lookup"><span data-stu-id="d05eb-137">**createdDateTime** is set in the future.</span></span>
* <span data-ttu-id="d05eb-138">**已正确指定 createdDateTime，\*\*\*\*但 channelCreationMode** 实例属性缺失或设置为无效值。</span><span class="sxs-lookup"><span data-stu-id="d05eb-138">**createdDateTime** is correctly specified but the **channelCreationMode** instance attribute is missing or set to an invalid value.</span></span>

## <a name="examples"></a><span data-ttu-id="d05eb-139">示例</span><span class="sxs-lookup"><span data-stu-id="d05eb-139">Examples</span></span>

### <a name="example-1-create-a-standard-channel"></a><span data-ttu-id="d05eb-140">示例 1：创建标准通道</span><span class="sxs-lookup"><span data-stu-id="d05eb-140">Example 1: Create a standard channel</span></span>

#### <a name="request"></a><span data-ttu-id="d05eb-141">请求</span><span class="sxs-lookup"><span data-stu-id="d05eb-141">Request</span></span>

<span data-ttu-id="d05eb-142">以下示例显示创建标准通道的请求。</span><span class="sxs-lookup"><span data-stu-id="d05eb-142">The following example shows a request to create a standard channel.</span></span>


# <a name="http"></a>[<span data-ttu-id="d05eb-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="d05eb-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_channel_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels
Content-type: application/json

{
  "displayName": "Architecture Discussion",
  "description": "This channel is where we debate all future architecture plans",
  "membershipType": "standard"
}
```
# <a name="c"></a>[<span data-ttu-id="d05eb-144">C#</span><span class="sxs-lookup"><span data-stu-id="d05eb-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-channel-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d05eb-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d05eb-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-channel-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d05eb-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d05eb-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-channel-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d05eb-147">Java</span><span class="sxs-lookup"><span data-stu-id="d05eb-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-channel-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="d05eb-148">响应</span><span class="sxs-lookup"><span data-stu-id="d05eb-148">Response</span></span>

<span data-ttu-id="d05eb-149">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="d05eb-149">The following example shows the response.</span></span>

> <span data-ttu-id="d05eb-150">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d05eb-150">**Note:** The response object shown here might be shortened for readability.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "name": "create_channel_from_group",
  "@odata.type": "microsoft.graph.channel"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 201

{
  "id": "19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2",
  "displayName": "Architecture Discussion",
  "description": "This channel is where we debate all future architecture plans"
}
```

### <a name="example-2-create-private-channel-on-behalf-of-user"></a><span data-ttu-id="d05eb-151">示例 2：代表用户创建私人频道</span><span class="sxs-lookup"><span data-stu-id="d05eb-151">Example 2: Create private channel on behalf of user</span></span>

#### <a name="request"></a><span data-ttu-id="d05eb-152">请求</span><span class="sxs-lookup"><span data-stu-id="d05eb-152">Request</span></span>

<span data-ttu-id="d05eb-153">以下示例显示创建私人频道和将用户添加为团队所有者的请求。</span><span class="sxs-lookup"><span data-stu-id="d05eb-153">The following example shows a request to create a private channel and add a user as an team owner.</span></span>


# <a name="http"></a>[<span data-ttu-id="d05eb-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="d05eb-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_private_channel_with_member"
}-->

```http
POST https://graph.microsoft.com/beta/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels
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
           "user@odata.bind":"https://graph.microsoft.com/beta/users('62855810-484b-4823-9e01-60667f8b12ae')",
           "roles":["owner"]
        }
     ]
}
```
# <a name="c"></a>[<span data-ttu-id="d05eb-155">C#</span><span class="sxs-lookup"><span data-stu-id="d05eb-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-private-channel-with-member-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d05eb-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d05eb-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-private-channel-with-member-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d05eb-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d05eb-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-private-channel-with-member-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d05eb-158">Java</span><span class="sxs-lookup"><span data-stu-id="d05eb-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-private-channel-with-member-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="d05eb-159">响应</span><span class="sxs-lookup"><span data-stu-id="d05eb-159">Response</span></span>

<span data-ttu-id="d05eb-160">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="d05eb-160">The following example shows the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "name": "create_private_channel_with_member",
  "@odata.type": "microsoft.graph.channel"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 201

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('57fb72d0-d811-46f4-8947-305e6072eaa5')/channels/$entity",
    "id": "19:33b76eea88574bd1969dca37e2b7a819@thread.skype",
    "displayName": "My First Private Channel",
    "description": "This is my first private channels",
    "isFavoriteByDefault": null,
    "email": "",
    "webUrl": "https://teams.microsoft.com/l/channel/19:33b76eea88574bd1969dca37e2b7a819@thread.skype/My%20First%20Private%20Channel?groupId=57fb72d0-d811-46f4-8947-305e6072eaa5&tenantId=0fddfdc5-f319-491f-a514-be1bc1bf9ddc",
    "membershipType": "private"
}
```

### <a name="example-3-create-a-channel-in-migration-mode"></a><span data-ttu-id="d05eb-161">示例 3：在迁移模式下创建通道</span><span class="sxs-lookup"><span data-stu-id="d05eb-161">Example 3: Create a channel in migration mode</span></span>

#### <a name="request"></a><span data-ttu-id="d05eb-162">请求</span><span class="sxs-lookup"><span data-stu-id="d05eb-162">Request</span></span>

<span data-ttu-id="d05eb-163">以下示例演示如何创建将用于导入邮件的通道。</span><span class="sxs-lookup"><span data-stu-id="d05eb-163">The following example shows how to create a channel that will be used for importing messages.</span></span>


<!-- {
  "blockType": "request",
  "name": "create_channel_for_migration"
}-->

```http
POST https://graph.microsoft.com/beta/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels
Content-Type: application/json

{
  "@microsoft.graph.channelCreationMode": "migration",
  "displayName": "Import_150958_99z",
  "description": "Import_150958_99z",
  "createdDateTime": "2020-03-14T11:22:17.067Z"
}
```


#### <a name="response"></a><span data-ttu-id="d05eb-164">响应</span><span class="sxs-lookup"><span data-stu-id="d05eb-164">Response</span></span>

<span data-ttu-id="d05eb-165">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="d05eb-165">The following example shows the response.</span></span> <span data-ttu-id="d05eb-166">响应中的 Content-Location 标头指定要预配的频道的路径。</span><span class="sxs-lookup"><span data-stu-id="d05eb-166">The Content-Location header in the response specifies the path to the channel that is being provisioned.</span></span>
<span data-ttu-id="d05eb-167">设置后，此通道可用于 [导入邮件](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams)。</span><span class="sxs-lookup"><span data-stu-id="d05eb-167">Once provisioned, this channel can be used for [importing messages](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams).</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "name": "create_channel_for_migration",
  "@odata.type": "microsoft.graph.channel"
} -->

```http
HTTP/1.1 201 Created
Location: /teams('57fb72d0-d811-46f4-8947-305e6072eaa5')/channels('19:4b6bed8d24574f6a9e436813cb2617d8@thread.tacv2')

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('57fb72d0-d811-46f4-8947-305e6072eaa5')/channels/$entity",
    "id": "19:987c7a9fbe6447ccb3ea31bcded5c75c@thread.tacv2",
    "createdDateTime": null,
    "displayName": "Import_150958_99z",
    "description": "Import_150958_99z",
    "isFavoriteByDefault": null,
    "email": null,
    "webUrl": null,
    "membershipType": null,
    "moderationSettings": null
}
```

### <a name="example-4-create-standard-channel-with-moderation-settings"></a><span data-ttu-id="d05eb-168">示例 4：使用审核设置创建标准频道</span><span class="sxs-lookup"><span data-stu-id="d05eb-168">Example 4: Create standard channel with moderation settings</span></span>

#### <a name="request"></a><span data-ttu-id="d05eb-169">请求</span><span class="sxs-lookup"><span data-stu-id="d05eb-169">Request</span></span>

<span data-ttu-id="d05eb-170">下面的示例展示了使用审核设置创建标准频道的请求。</span><span class="sxs-lookup"><span data-stu-id="d05eb-170">The following example shows a request to create a standard channel with moderation settings.</span></span> <span data-ttu-id="d05eb-171">只能对标准通道执行此操作。</span><span class="sxs-lookup"><span data-stu-id="d05eb-171">This operation can only be performed for a standard channel.</span></span>


# <a name="http"></a>[<span data-ttu-id="d05eb-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="d05eb-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_channel_with_moderation_settings"
}-->

```http
POST https://graph.microsoft.com/beta/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels
Content-type: application/json

{
    "displayName": "TestChannelModeration",
    "description": "Test channel moderation.",
    "membershipType": "standard",
    "moderationSettings": {
        "userNewMessageRestriction": "everyoneExceptGuests",
        "replyRestriction": "everyone",
        "allowNewMessageFromBots": true,
        "allowNewMessageFromConnectors": true
    }
}
```
# <a name="c"></a>[<span data-ttu-id="d05eb-173">C#</span><span class="sxs-lookup"><span data-stu-id="d05eb-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-channel-with-moderation-settings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d05eb-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d05eb-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-channel-with-moderation-settings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d05eb-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d05eb-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-channel-with-moderation-settings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d05eb-176">Java</span><span class="sxs-lookup"><span data-stu-id="d05eb-176">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-channel-with-moderation-settings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="d05eb-177">响应</span><span class="sxs-lookup"><span data-stu-id="d05eb-177">Response</span></span>

<span data-ttu-id="d05eb-178">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="d05eb-178">The following example shows the response.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('57fb72d0-d811-46f4-8947-305e6072eaa5')/channels/$entity",
    "id": "19:12b76eea88574bd1969dca37e2b7a819@thread.skype",
    "displayName": "My First Private Channel",
    "description": "This is my first private channels",
    "isFavoriteByDefault": null,
    "email": "",
    "webUrl": "https://teams.microsoft.com/l/channel/19:12b76eea88574bd1969dca37e2b7a819@thread.skype/My%20First%20Private%20Channel?groupId=57fb72d0-d811-46f4-8947-305e6072eaa5&tenantId=0fddfdc5-f319-491f-a514-be1bc1bf9ddc",
    "membershipType": "private"
}
```

## <a name="see-also"></a><span data-ttu-id="d05eb-179">另请参阅</span><span class="sxs-lookup"><span data-stu-id="d05eb-179">See also</span></span>

* [<span data-ttu-id="d05eb-180">频道的完整迁移</span><span class="sxs-lookup"><span data-stu-id="d05eb-180">Complete migration for a channel</span></span>](channel-completemigration.md)
* [<span data-ttu-id="d05eb-181">使用 Microsoft Graph 将第三方平台消息导入 Teams</span><span class="sxs-lookup"><span data-stu-id="d05eb-181">Import third-party platform messages to Teams using Microsoft Graph</span></span>](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams)
* [<span data-ttu-id="d05eb-182">创建团队</span><span class="sxs-lookup"><span data-stu-id="d05eb-182">Create team</span></span>](team-post.md)

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
