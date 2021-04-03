---
title: 创建频道
description: 在团队中创建新频道，如请求正文中指定。
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: ac06a2898662ce13db588ea0f243f6d3eea65805
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508446"
---
# <a name="create-channel"></a><span data-ttu-id="85588-103">创建频道</span><span class="sxs-lookup"><span data-stu-id="85588-103">Create channel</span></span>

<span data-ttu-id="85588-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85588-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="85588-105">在团队 [中创建新](../resources/channel.md) 频道，如请求正文中指定。</span><span class="sxs-lookup"><span data-stu-id="85588-105">Create a new [channel](../resources/channel.md) in a team, as specified in the request body.</span></span>

## <a name="permissions"></a><span data-ttu-id="85588-106">权限</span><span class="sxs-lookup"><span data-stu-id="85588-106">Permissions</span></span>

<span data-ttu-id="85588-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="85588-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85588-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="85588-109">Permission type</span></span>      | <span data-ttu-id="85588-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="85588-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="85588-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="85588-111">Delegated (work or school account)</span></span> | <span data-ttu-id="85588-112">Channel.Create、Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85588-112">Channel.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="85588-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="85588-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85588-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="85588-114">Not supported.</span></span>    |
|<span data-ttu-id="85588-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="85588-115">Application</span></span> | <span data-ttu-id="85588-116">Channel.Create.Group\*、Channel.Create、Teamwork.Migrate.All、Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="85588-116">Channel.Create.Group\*, Channel.Create, Teamwork.Migrate.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="85588-117">**备注：** 标有 \* 的权限使用 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="85588-117">**Notes**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>
>
> <span data-ttu-id="85588-118">此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="85588-118">This API supports admin permissions.</span></span> <span data-ttu-id="85588-119">全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的团队。</span><span class="sxs-lookup"><span data-stu-id="85588-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>
>
> <span data-ttu-id="85588-120">将来，Microsoft 可能会要求你或你的客户根据使用团队合作导入的数据量支付额外的费用。Migrate.All 和/或[迁移 API。](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams)</span><span class="sxs-lookup"><span data-stu-id="85588-120">In the future, Microsoft may require you or your customers to pay additional fees based on the amount of data imported using Teamwork.Migrate.All and/or [migration APIs](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams).</span></span>

## <a name="http-request"></a><span data-ttu-id="85588-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="85588-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{team-id}/channels
```

## <a name="request-headers"></a><span data-ttu-id="85588-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="85588-122">Request headers</span></span>

| <span data-ttu-id="85588-123">标头</span><span class="sxs-lookup"><span data-stu-id="85588-123">Header</span></span>       | <span data-ttu-id="85588-124">值</span><span class="sxs-lookup"><span data-stu-id="85588-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="85588-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="85588-125">Authorization</span></span>  | <span data-ttu-id="85588-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="85588-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="85588-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="85588-128">Content-Type</span></span>  | <span data-ttu-id="85588-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="85588-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="85588-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="85588-131">Request body</span></span>

<span data-ttu-id="85588-132">在请求正文中，提供 [channel](../resources/channel.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="85588-132">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="85588-133">响应</span><span class="sxs-lookup"><span data-stu-id="85588-133">Response</span></span>

<span data-ttu-id="85588-134">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [channel](../resources/channel.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="85588-134">If successful, this method returns a `201 Created` response code and a [channel](../resources/channel.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="85588-135">示例</span><span class="sxs-lookup"><span data-stu-id="85588-135">Examples</span></span>

### <a name="example-1-create-a-standard-channel"></a><span data-ttu-id="85588-136">示例 1：创建标准通道</span><span class="sxs-lookup"><span data-stu-id="85588-136">Example 1: Create a standard channel</span></span>
#### <a name="request"></a><span data-ttu-id="85588-137">请求</span><span class="sxs-lookup"><span data-stu-id="85588-137">Request</span></span>

<span data-ttu-id="85588-138">以下示例显示创建标准通道的请求。</span><span class="sxs-lookup"><span data-stu-id="85588-138">The following example shows a request to create a standard channel.</span></span>


# <a name="http"></a>[<span data-ttu-id="85588-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="85588-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_channel_from_group"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels
Content-type: application/json

{
  "displayName": "Architecture Discussion",
  "description": "This channel is where we debate all future architecture plans",
  "membershipType": "standard"
}
```
# <a name="c"></a>[<span data-ttu-id="85588-140">C#</span><span class="sxs-lookup"><span data-stu-id="85588-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-channel-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="85588-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="85588-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-channel-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="85588-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="85588-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-channel-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="85588-143">Java</span><span class="sxs-lookup"><span data-stu-id="85588-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-channel-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="85588-144">响应</span><span class="sxs-lookup"><span data-stu-id="85588-144">Response</span></span>

<span data-ttu-id="85588-145">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="85588-145">The following example shows the response.</span></span>

> <span data-ttu-id="85588-146">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="85588-146">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
}-->

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

### <a name="example-2-create-private-channel-on-behalf-of-user"></a><span data-ttu-id="85588-147">示例 2：代表用户创建私人频道</span><span class="sxs-lookup"><span data-stu-id="85588-147">Example 2: Create private channel on behalf of user</span></span>

#### <a name="request"></a><span data-ttu-id="85588-148">请求</span><span class="sxs-lookup"><span data-stu-id="85588-148">Request</span></span>

<span data-ttu-id="85588-149">以下示例显示创建私人频道和将用户添加为团队所有者的请求。</span><span class="sxs-lookup"><span data-stu-id="85588-149">The following example shows a request to create a private channel and add a user as an team owner.</span></span>



# <a name="http"></a>[<span data-ttu-id="85588-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="85588-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_channel_from_user"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels
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
           "user@odata.bind":"https://graph.microsoft.com/v1.0/users('62855810-484b-4823-9e01-60667f8b12ae')",
           "roles":["owner"]
        }
     ]
}
```
# <a name="c"></a>[<span data-ttu-id="85588-151">C#</span><span class="sxs-lookup"><span data-stu-id="85588-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-channel-from-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="85588-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="85588-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-channel-from-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="85588-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="85588-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-channel-from-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="85588-154">Java</span><span class="sxs-lookup"><span data-stu-id="85588-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-channel-from-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---




#### <a name="response"></a><span data-ttu-id="85588-155">响应</span><span class="sxs-lookup"><span data-stu-id="85588-155">Response</span></span>

<span data-ttu-id="85588-156">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="85588-156">The following example shows the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
}-->

```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 201

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('57fb72d0-d811-46f4-8947-305e6072eaa5')/channels/$entity",
    "id": "19:33b76eea88574bd1969dca37e2b7a819@thread.skype",
    "displayName": "My First Private Channel",
    "description": "This is my first private channels",
    "isFavoriteByDefault": null,
    "email": "",
    "webUrl": "https://teams.microsoft.com/l/channel/19:33b76eea88574bd1969dca37e2b7a819@thread.skype/My%20First%20Private%20Channel?groupId=57fb72d0-d811-46f4-8947-305e6072eaa5&tenantId=0fddfdc5-f319-491f-a514-be1bc1bf9ddc",
    "membershipType": "private"
}
```

### <a name="example-3-create-a-channel-in-migration-mode"></a><span data-ttu-id="85588-157">示例 3：在迁移模式下创建通道</span><span class="sxs-lookup"><span data-stu-id="85588-157">Example 3: Create a channel in migration mode</span></span>

#### <a name="request"></a><span data-ttu-id="85588-158">请求</span><span class="sxs-lookup"><span data-stu-id="85588-158">Request</span></span>

<span data-ttu-id="85588-159">以下示例演示如何创建将用于导入邮件的通道。</span><span class="sxs-lookup"><span data-stu-id="85588-159">The following example shows how to create a channel that will be used for importing messages.</span></span>



# <a name="http"></a>[<span data-ttu-id="85588-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="85588-160">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_channel_for_migration"
}-->

```http
POST https://graph.microsoft.com/v1.0/teams/57fb72d0-d811-46f4-8947-305e6072eaa5/channels
Content-Type: application/json

{
  "@microsoft.graph.channelCreationMode": "migration",
  "displayName": "Import_150958_99z",
  "description": "Import_150958_99z",
  "createdDateTime": "2020-03-14T11:22:17.067Z"
}
```
# <a name="c"></a>[<span data-ttu-id="85588-161">C#</span><span class="sxs-lookup"><span data-stu-id="85588-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-channel-for-migration-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="85588-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="85588-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-channel-for-migration-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="85588-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="85588-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-channel-for-migration-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="85588-164">Java</span><span class="sxs-lookup"><span data-stu-id="85588-164">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-channel-for-migration-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="85588-165">响应</span><span class="sxs-lookup"><span data-stu-id="85588-165">Response</span></span>

<span data-ttu-id="85588-166">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="85588-166">The following example shows the response.</span></span> <span data-ttu-id="85588-167">响应中的 Content-Location 标头指定要预配的频道的路径。</span><span class="sxs-lookup"><span data-stu-id="85588-167">The Content-Location header in the response specifies the path to the channel that is being provisioned.</span></span>
<span data-ttu-id="85588-168">设置后，此通道可用于 [导入邮件](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams)。</span><span class="sxs-lookup"><span data-stu-id="85588-168">Once provisioned, this channel can be used for [importing messages](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams).</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#teams('57fb72d0-d811-46f4-8947-305e6072eaa5')/channels/$entity",
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
