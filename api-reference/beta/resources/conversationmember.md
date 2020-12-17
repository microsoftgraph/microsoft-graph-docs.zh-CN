---
title: conversationMember 资源类型
description: 表示对话中的用户。
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7f6b24b65a6ae25f8a05bf067659c04d49c06d24
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706058"
---
# <a name="conversationmember-resource-type"></a><span data-ttu-id="25499-103">conversationMember 资源类型</span><span class="sxs-lookup"><span data-stu-id="25499-103">conversationMember resource type</span></span>

<span data-ttu-id="25499-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="25499-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25499-105">表示[聊天](chat.md)或[频道](channel.md)中的用户。</span><span class="sxs-lookup"><span data-stu-id="25499-105">Represents a user in a [chat](chat.md) or a [channel](channel.md).</span></span>
<span data-ttu-id="25499-106">另请参阅 [aadUserConversationMember](aaduserconversationmember.md)。</span><span class="sxs-lookup"><span data-stu-id="25499-106">See also [aadUserConversationMember](aaduserconversationmember.md).</span></span>

## <a name="methods"></a><span data-ttu-id="25499-107">方法</span><span class="sxs-lookup"><span data-stu-id="25499-107">Methods</span></span>

| <span data-ttu-id="25499-108">方法</span><span class="sxs-lookup"><span data-stu-id="25499-108">Method</span></span>       | <span data-ttu-id="25499-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="25499-109">Return Type</span></span>  |<span data-ttu-id="25499-110">说明</span><span class="sxs-lookup"><span data-stu-id="25499-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="25499-111">列出团队成员</span><span class="sxs-lookup"><span data-stu-id="25499-111">List team members</span></span>](../api/team-list-members.md)|<span data-ttu-id="25499-112">[conversationMember](../resources/conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="25499-112">[conversationMember](../resources/conversationmember.md) collection</span></span>|<span data-ttu-id="25499-113">获取此团队中的成员列表。</span><span class="sxs-lookup"><span data-stu-id="25499-113">Get the list of members in the team.</span></span>|
|[<span data-ttu-id="25499-114">获取团队成员</span><span class="sxs-lookup"><span data-stu-id="25499-114">Get team member</span></span>](../api/team-get-members.md) | <span data-ttu-id="25499-115">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="25499-115">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="25499-116">获取团队中的成员。</span><span class="sxs-lookup"><span data-stu-id="25499-116">Get a member in the team.</span></span>|
|[<span data-ttu-id="25499-117">添加团队成员</span><span class="sxs-lookup"><span data-stu-id="25499-117">Add team member</span></span>](../api/team-post-members.md)|[<span data-ttu-id="25499-118">conversationMember</span><span class="sxs-lookup"><span data-stu-id="25499-118">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="25499-119">向团队中添加新成员。</span><span class="sxs-lookup"><span data-stu-id="25499-119">Add a new member to the team.</span></span>|
|[<span data-ttu-id="25499-120">批量添加团队成员</span><span class="sxs-lookup"><span data-stu-id="25499-120">Add team members in bulk</span></span>](../api/conversationmembers-add.md)|<span data-ttu-id="25499-121">[actionResultPart](../resources/actionresultpart.md) 集合</span><span class="sxs-lookup"><span data-stu-id="25499-121">[actionResultPart](../resources/actionresultpart.md) collection</span></span>|<span data-ttu-id="25499-122">在单个请求中将多个成员添加到团队中。</span><span class="sxs-lookup"><span data-stu-id="25499-122">Add multiple members to the team in a single request.</span></span>|
|[<span data-ttu-id="25499-123">更新团队成员的角色</span><span class="sxs-lookup"><span data-stu-id="25499-123">Update team member's role</span></span>](../api/team-update-members.md)|[<span data-ttu-id="25499-124">conversationMember</span><span class="sxs-lookup"><span data-stu-id="25499-124">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="25499-125">将成员更改为所有者或返回为常规成员。</span><span class="sxs-lookup"><span data-stu-id="25499-125">Change a member to an owner or back to a regular member.</span></span>|
|[<span data-ttu-id="25499-126">删除团队成员</span><span class="sxs-lookup"><span data-stu-id="25499-126">Remove team member</span></span>](../api/team-delete-members.md)|<span data-ttu-id="25499-127">无</span><span class="sxs-lookup"><span data-stu-id="25499-127">None</span></span>|<span data-ttu-id="25499-128">删除团队中的一个现有成员。</span><span class="sxs-lookup"><span data-stu-id="25499-128">Remove an existing member from the team.</span></span>|
|[<span data-ttu-id="25499-129">列出频道成员</span><span class="sxs-lookup"><span data-stu-id="25499-129">List channel members</span></span>](../api/channel-list-members.md) | <span data-ttu-id="25499-130">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="25499-130">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="25499-131">获取频道中所有成员的列表。</span><span class="sxs-lookup"><span data-stu-id="25499-131">Get the list of all members in a channel.</span></span>|
|[<span data-ttu-id="25499-132">获取频道成员</span><span class="sxs-lookup"><span data-stu-id="25499-132">Get channel member</span></span>](../api/channel-get-members.md) | <span data-ttu-id="25499-133">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="25499-133">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="25499-134">获取频道中的成员。</span><span class="sxs-lookup"><span data-stu-id="25499-134">Get a member in a channel.</span></span>|
|[<span data-ttu-id="25499-135">创建频道成员</span><span class="sxs-lookup"><span data-stu-id="25499-135">Create channel member</span></span>](../api/channel-post-members.md) | [<span data-ttu-id="25499-136">conversationMember</span><span class="sxs-lookup"><span data-stu-id="25499-136">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="25499-137">向频道添加成员。</span><span class="sxs-lookup"><span data-stu-id="25499-137">Add a member to a channel.</span></span> <span data-ttu-id="25499-138">仅支持 membershipType 为 `private` 的 `channel`。</span><span class="sxs-lookup"><span data-stu-id="25499-138">Only supported for `channel`with membershipType of `private`.</span></span>|
|[<span data-ttu-id="25499-139">更新频道成员角色</span><span class="sxs-lookup"><span data-stu-id="25499-139">Update channel member's role</span></span>](../api/channel-update-members.md) | [<span data-ttu-id="25499-140">conversationMember</span><span class="sxs-lookup"><span data-stu-id="25499-140">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="25499-141">更新频道成员的属性。</span><span class="sxs-lookup"><span data-stu-id="25499-141">Update the properties of a member of the channel.</span></span> <span data-ttu-id="25499-142">仅支持 membershipType 为 `private` 的频道。</span><span class="sxs-lookup"><span data-stu-id="25499-142">Only supported for channel with membershipType of `private`.</span></span>|
|[<span data-ttu-id="25499-143">删除频道成员</span><span class="sxs-lookup"><span data-stu-id="25499-143">Remove channel member</span></span>](../api/channel-delete-members.md) | <span data-ttu-id="25499-144">无</span><span class="sxs-lookup"><span data-stu-id="25499-144">None</span></span> | <span data-ttu-id="25499-145">从频道中删除一个成员。</span><span class="sxs-lookup"><span data-stu-id="25499-145">Delete a member from a channel.</span></span> <span data-ttu-id="25499-146">仅支持用于 `private` 的 `channelType`。</span><span class="sxs-lookup"><span data-stu-id="25499-146">Only supported for `channelType` of `private`.</span></span>|
|[<span data-ttu-id="25499-147">列出聊天成员</span><span class="sxs-lookup"><span data-stu-id="25499-147">List chat members</span></span>](../api/chat-list-members.md) | <span data-ttu-id="25499-148">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="25499-148">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="25499-149">获取聊天中所有成员的列表。</span><span class="sxs-lookup"><span data-stu-id="25499-149">Get the list of all members in a chat.</span></span>|
|[<span data-ttu-id="25499-150">获取聊天成员</span><span class="sxs-lookup"><span data-stu-id="25499-150">Get chat member</span></span>](../api/chat-get-members.md) | [<span data-ttu-id="25499-151">conversationMember</span><span class="sxs-lookup"><span data-stu-id="25499-151">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="25499-152">获取聊天中的成员。</span><span class="sxs-lookup"><span data-stu-id="25499-152">Get a member in a chat.</span></span>|
|[<span data-ttu-id="25499-153">添加聊天成员</span><span class="sxs-lookup"><span data-stu-id="25499-153">Add chat member</span></span>](../api/chat-post-members.md) | <span data-ttu-id="25499-154">位置标头</span><span class="sxs-lookup"><span data-stu-id="25499-154">Location header</span></span> | <span data-ttu-id="25499-155">向聊天添加成员。</span><span class="sxs-lookup"><span data-stu-id="25499-155">Add a member to a chat.</span></span>| 

## <a name="properties"></a><span data-ttu-id="25499-156">属性</span><span class="sxs-lookup"><span data-stu-id="25499-156">Properties</span></span>

| <span data-ttu-id="25499-157">属性</span><span class="sxs-lookup"><span data-stu-id="25499-157">Property</span></span>   | <span data-ttu-id="25499-158">类型</span><span class="sxs-lookup"><span data-stu-id="25499-158">Type</span></span> |<span data-ttu-id="25499-159">说明</span><span class="sxs-lookup"><span data-stu-id="25499-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="25499-160">id</span><span class="sxs-lookup"><span data-stu-id="25499-160">id</span></span>|<span data-ttu-id="25499-161">字符串</span><span class="sxs-lookup"><span data-stu-id="25499-161">String</span></span>| <span data-ttu-id="25499-162">只读。</span><span class="sxs-lookup"><span data-stu-id="25499-162">Read-only.</span></span> <span data-ttu-id="25499-163">用户的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="25499-163">Unique ID of the user.</span></span>|
|<span data-ttu-id="25499-164">displayName</span><span class="sxs-lookup"><span data-stu-id="25499-164">displayName</span></span>| <span data-ttu-id="25499-165">string</span><span class="sxs-lookup"><span data-stu-id="25499-165">string</span></span> | <span data-ttu-id="25499-166">用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="25499-166">The display name of the user.</span></span> |
|<span data-ttu-id="25499-167">角色</span><span class="sxs-lookup"><span data-stu-id="25499-167">roles</span></span>| <span data-ttu-id="25499-168">string 集合</span><span class="sxs-lookup"><span data-stu-id="25499-168">string collection</span></span> | <span data-ttu-id="25499-169">该用户的角色。</span><span class="sxs-lookup"><span data-stu-id="25499-169">The roles for that user.</span></span> |
|<span data-ttu-id="25499-170">visibleHistoryStartDateTime</span><span class="sxs-lookup"><span data-stu-id="25499-170">visibleHistoryStartDateTime</span></span>| <span data-ttu-id="25499-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25499-171">DateTimeOffset</span></span> | <span data-ttu-id="25499-172">表示对话历史记录与对话成员共享多远的时间戳。</span><span class="sxs-lookup"><span data-stu-id="25499-172">The timestamp denoting how far back a conversation's history is shared with the conversation member.</span></span> <span data-ttu-id="25499-173">此属性仅对聊天成员可设置。</span><span class="sxs-lookup"><span data-stu-id="25499-173">This property is settable only for members of a chat.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="25499-174">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="25499-174">JSON representation</span></span>

<span data-ttu-id="25499-175">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="25499-175">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.conversationMember",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.conversationMember",
  "id": "String (identifier)",
  "roles": [
    "String"
  ],
  "displayName": "String",
  "visibleHistoryStartDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conversationMember resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


