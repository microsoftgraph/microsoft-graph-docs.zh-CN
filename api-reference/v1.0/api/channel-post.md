---
title: 创建频道
description: 在团队中创建新频道，如请求正文中指定。
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 7ab9a2d0bdd204e77b9bc149860e9fdfab9d2fcf
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51202693"
---
# <a name="create-channel"></a><span data-ttu-id="01346-103">创建频道</span><span class="sxs-lookup"><span data-stu-id="01346-103">Create channel</span></span>

<span data-ttu-id="01346-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01346-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="01346-105">在团队 [中创建新](../resources/channel.md) 频道，如请求正文中指定。</span><span class="sxs-lookup"><span data-stu-id="01346-105">Create a new [channel](../resources/channel.md) in a team, as specified in the request body.</span></span>

## <a name="permissions"></a><span data-ttu-id="01346-106">权限</span><span class="sxs-lookup"><span data-stu-id="01346-106">Permissions</span></span>

<span data-ttu-id="01346-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="01346-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01346-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="01346-109">Permission type</span></span>      | <span data-ttu-id="01346-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="01346-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="01346-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="01346-111">Delegated (work or school account)</span></span> | <span data-ttu-id="01346-112">Channel.Create、Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01346-112">Channel.Create, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="01346-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="01346-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01346-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="01346-114">Not supported.</span></span>    |
|<span data-ttu-id="01346-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="01346-115">Application</span></span> | <span data-ttu-id="01346-116">Channel.Create.Group\*、Channel.Create、Teamwork.Migrate.All、Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01346-116">Channel.Create.Group\*, Channel.Create, Teamwork.Migrate.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="01346-117">**备注：** 标有 \* 的权限使用 [特定于资源的同意]( https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="01346-117">**Notes**: Permissions marked with \* use [resource-specific consent]( https://aka.ms/teams-rsc).</span></span>
>
> <span data-ttu-id="01346-118">此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="01346-118">This API supports admin permissions.</span></span> <span data-ttu-id="01346-119">全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的团队。</span><span class="sxs-lookup"><span data-stu-id="01346-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>
>
> <span data-ttu-id="01346-120">将来，Microsoft 可能会要求你或你的客户根据使用团队合作导入的数据量支付额外的费用。Migrate.All 和/或[迁移 API。](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams)</span><span class="sxs-lookup"><span data-stu-id="01346-120">In the future, Microsoft may require you or your customers to pay additional fees based on the amount of data imported using Teamwork.Migrate.All and/or [migration APIs](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams).</span></span>

## <a name="http-request"></a><span data-ttu-id="01346-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="01346-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{team-id}/channels
```

## <a name="request-headers"></a><span data-ttu-id="01346-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="01346-122">Request headers</span></span>

| <span data-ttu-id="01346-123">标头</span><span class="sxs-lookup"><span data-stu-id="01346-123">Header</span></span>       | <span data-ttu-id="01346-124">值</span><span class="sxs-lookup"><span data-stu-id="01346-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="01346-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="01346-125">Authorization</span></span>  | <span data-ttu-id="01346-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="01346-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="01346-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="01346-128">Content-Type</span></span>  | <span data-ttu-id="01346-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="01346-p104">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="01346-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="01346-131">Request body</span></span>

<span data-ttu-id="01346-132">在请求正文中，提供 [channel](../resources/channel.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="01346-132">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="01346-133">响应</span><span class="sxs-lookup"><span data-stu-id="01346-133">Response</span></span>

<span data-ttu-id="01346-134">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [channel](../resources/channel.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="01346-134">If successful, this method returns a `201 Created` response code and a [channel](../resources/channel.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="01346-135">示例</span><span class="sxs-lookup"><span data-stu-id="01346-135">Examples</span></span>

### <a name="example-1-create-a-standard-channel"></a><span data-ttu-id="01346-136">示例 1：创建标准通道</span><span class="sxs-lookup"><span data-stu-id="01346-136">Example 1: Create a standard channel</span></span>
#### <a name="request"></a><span data-ttu-id="01346-137">请求</span><span class="sxs-lookup"><span data-stu-id="01346-137">Request</span></span>

<span data-ttu-id="01346-138">以下示例显示创建标准通道的请求。</span><span class="sxs-lookup"><span data-stu-id="01346-138">The following example shows a request to create a standard channel.</span></span>

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


#### <a name="response"></a><span data-ttu-id="01346-139">响应</span><span class="sxs-lookup"><span data-stu-id="01346-139">Response</span></span>

<span data-ttu-id="01346-140">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="01346-140">The following example shows the response.</span></span>

> <span data-ttu-id="01346-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="01346-141">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-create-private-channel-on-behalf-of-user"></a><span data-ttu-id="01346-142">示例 2：代表用户创建私人频道</span><span class="sxs-lookup"><span data-stu-id="01346-142">Example 2: Create private channel on behalf of user</span></span>

#### <a name="request"></a><span data-ttu-id="01346-143">请求</span><span class="sxs-lookup"><span data-stu-id="01346-143">Request</span></span>

<span data-ttu-id="01346-144">以下示例显示创建私人频道和将用户添加为团队所有者的请求。</span><span class="sxs-lookup"><span data-stu-id="01346-144">The following example shows a request to create a private channel and add a user as an team owner.</span></span>


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



#### <a name="response"></a><span data-ttu-id="01346-145">响应</span><span class="sxs-lookup"><span data-stu-id="01346-145">Response</span></span>

<span data-ttu-id="01346-146">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="01346-146">The following example shows the response.</span></span>

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

### <a name="example-3-create-a-channel-in-migration-mode"></a><span data-ttu-id="01346-147">示例 3：在迁移模式下创建通道</span><span class="sxs-lookup"><span data-stu-id="01346-147">Example 3: Create a channel in migration mode</span></span>

#### <a name="request"></a><span data-ttu-id="01346-148">请求</span><span class="sxs-lookup"><span data-stu-id="01346-148">Request</span></span>

<span data-ttu-id="01346-149">以下示例演示如何创建将用于导入邮件的通道。</span><span class="sxs-lookup"><span data-stu-id="01346-149">The following example shows how to create a channel that will be used for importing messages.</span></span>


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


#### <a name="response"></a><span data-ttu-id="01346-150">响应</span><span class="sxs-lookup"><span data-stu-id="01346-150">Response</span></span>

<span data-ttu-id="01346-151">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="01346-151">The following example shows the response.</span></span> <span data-ttu-id="01346-152">响应中的 Content-Location 标头指定要预配的频道的路径。</span><span class="sxs-lookup"><span data-stu-id="01346-152">The Content-Location header in the response specifies the path to the channel that is being provisioned.</span></span>
<span data-ttu-id="01346-153">设置后，此通道可用于 [导入邮件](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams)。</span><span class="sxs-lookup"><span data-stu-id="01346-153">Once provisioned, this channel can be used for [importing messages](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams).</span></span>
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
