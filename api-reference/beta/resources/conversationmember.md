---
title: conversationMember 资源类型
description: 表示对话中的用户。
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a3ff911392d019bb387298dc2fb8252b222ed520
ms.sourcegitcommit: 0d4377b0153bc339ab7b3b1a6ee4d52848b622d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2020
ms.locfileid: "49714135"
---
# <a name="conversationmember-resource-type"></a><span data-ttu-id="77788-103">conversationMember 资源类型</span><span class="sxs-lookup"><span data-stu-id="77788-103">conversationMember resource type</span></span>

<span data-ttu-id="77788-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77788-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77788-105">表示团队、 [频道](team.md) 或 [聊天](channel.md) 中的 [用户](chat.md)。</span><span class="sxs-lookup"><span data-stu-id="77788-105">Represents a user in a [team](team.md) or a [channel](channel.md) or a [chat](chat.md).</span></span>
<span data-ttu-id="77788-106">另请参阅 [aadUserConversationMember](aaduserconversationmember.md)。</span><span class="sxs-lookup"><span data-stu-id="77788-106">See also [aadUserConversationMember](aaduserconversationmember.md).</span></span>

## <a name="methods"></a><span data-ttu-id="77788-107">方法</span><span class="sxs-lookup"><span data-stu-id="77788-107">Methods</span></span>

| <span data-ttu-id="77788-108">方法</span><span class="sxs-lookup"><span data-stu-id="77788-108">Method</span></span>       | <span data-ttu-id="77788-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="77788-109">Return Type</span></span>  |<span data-ttu-id="77788-110">说明</span><span class="sxs-lookup"><span data-stu-id="77788-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="77788-111">列出团队成员</span><span class="sxs-lookup"><span data-stu-id="77788-111">List team members</span></span>](../api/team-list-members.md)|<span data-ttu-id="77788-112">[conversationMember](../resources/conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="77788-112">[conversationMember](../resources/conversationmember.md) collection</span></span>|<span data-ttu-id="77788-113">获取此团队中的成员列表。</span><span class="sxs-lookup"><span data-stu-id="77788-113">Get the list of members in the team.</span></span>|
|[<span data-ttu-id="77788-114">添加团队成员</span><span class="sxs-lookup"><span data-stu-id="77788-114">Add team member</span></span>](../api/team-post-members.md)|[<span data-ttu-id="77788-115">conversationMember</span><span class="sxs-lookup"><span data-stu-id="77788-115">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="77788-116">向团队中添加新成员。</span><span class="sxs-lookup"><span data-stu-id="77788-116">Add a new member to the team.</span></span>|
|[<span data-ttu-id="77788-117">批量添加团队成员</span><span class="sxs-lookup"><span data-stu-id="77788-117">Add team members in bulk</span></span>](../api/conversationmembers-add.md)|<span data-ttu-id="77788-118">[actionResultPart](../resources/actionresultpart.md) 集合</span><span class="sxs-lookup"><span data-stu-id="77788-118">[actionResultPart](../resources/actionresultpart.md) collection</span></span>|<span data-ttu-id="77788-119">在单个请求中将多个成员添加到团队中。</span><span class="sxs-lookup"><span data-stu-id="77788-119">Add multiple members to the team in a single request.</span></span>|
|[<span data-ttu-id="77788-120">获取团队成员</span><span class="sxs-lookup"><span data-stu-id="77788-120">Get team member</span></span>](../api/team-get-members.md) | <span data-ttu-id="77788-121">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="77788-121">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="77788-122">获取团队中的成员。</span><span class="sxs-lookup"><span data-stu-id="77788-122">Get a member in the team.</span></span>|
|[<span data-ttu-id="77788-123">更新团队成员的角色</span><span class="sxs-lookup"><span data-stu-id="77788-123">Update team member's role</span></span>](../api/team-update-members.md)|[<span data-ttu-id="77788-124">conversationMember</span><span class="sxs-lookup"><span data-stu-id="77788-124">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="77788-125">将成员更改为所有者或返回为常规成员。</span><span class="sxs-lookup"><span data-stu-id="77788-125">Change a member to an owner or back to a regular member.</span></span>|
|[<span data-ttu-id="77788-126">删除团队成员</span><span class="sxs-lookup"><span data-stu-id="77788-126">Remove team member</span></span>](../api/team-delete-members.md)|<span data-ttu-id="77788-127">无</span><span class="sxs-lookup"><span data-stu-id="77788-127">None</span></span>|<span data-ttu-id="77788-128">删除团队中的一个现有成员。</span><span class="sxs-lookup"><span data-stu-id="77788-128">Remove an existing member from the team.</span></span>|
|[<span data-ttu-id="77788-129">列出频道成员</span><span class="sxs-lookup"><span data-stu-id="77788-129">List channel members</span></span>](../api/channel-list-members.md) | <span data-ttu-id="77788-130">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="77788-130">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="77788-131">获取频道中所有成员的列表。</span><span class="sxs-lookup"><span data-stu-id="77788-131">Get the list of all members in a channel.</span></span>|
|[<span data-ttu-id="77788-132">添加频道成员</span><span class="sxs-lookup"><span data-stu-id="77788-132">Add channel member</span></span>](../api/channel-post-members.md) | [<span data-ttu-id="77788-133">conversationMember</span><span class="sxs-lookup"><span data-stu-id="77788-133">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="77788-134">向频道添加成员。</span><span class="sxs-lookup"><span data-stu-id="77788-134">Add a member to a channel.</span></span> <span data-ttu-id="77788-135">仅支持 membershipType 为 `private` 的 `channel`。</span><span class="sxs-lookup"><span data-stu-id="77788-135">Only supported for `channel`with membershipType of `private`.</span></span>|
|[<span data-ttu-id="77788-136">获取频道成员</span><span class="sxs-lookup"><span data-stu-id="77788-136">Get channel member</span></span>](../api/channel-get-members.md) | <span data-ttu-id="77788-137">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="77788-137">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="77788-138">获取频道中的成员。</span><span class="sxs-lookup"><span data-stu-id="77788-138">Get a member in a channel.</span></span>|
|[<span data-ttu-id="77788-139">更新频道成员角色</span><span class="sxs-lookup"><span data-stu-id="77788-139">Update channel member's role</span></span>](../api/channel-update-members.md) | [<span data-ttu-id="77788-140">conversationMember</span><span class="sxs-lookup"><span data-stu-id="77788-140">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="77788-141">更新频道成员的属性。</span><span class="sxs-lookup"><span data-stu-id="77788-141">Update the properties of a member of the channel.</span></span> <span data-ttu-id="77788-142">仅支持 membershipType 为 `private` 的频道。</span><span class="sxs-lookup"><span data-stu-id="77788-142">Only supported for channel with membershipType of `private`.</span></span>|
|[<span data-ttu-id="77788-143">删除频道成员</span><span class="sxs-lookup"><span data-stu-id="77788-143">Remove channel member</span></span>](../api/channel-delete-members.md) | <span data-ttu-id="77788-144">无</span><span class="sxs-lookup"><span data-stu-id="77788-144">None</span></span> | <span data-ttu-id="77788-145">从频道中删除一个成员。</span><span class="sxs-lookup"><span data-stu-id="77788-145">Delete a member from a channel.</span></span> <span data-ttu-id="77788-146">仅支持用于 `private` 的 `channelType`。</span><span class="sxs-lookup"><span data-stu-id="77788-146">Only supported for `channelType` of `private`.</span></span>|
|[<span data-ttu-id="77788-147">列出聊天成员</span><span class="sxs-lookup"><span data-stu-id="77788-147">List chat members</span></span>](../api/chat-list-members.md) | <span data-ttu-id="77788-148">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="77788-148">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="77788-149">获取聊天中所有成员的列表。</span><span class="sxs-lookup"><span data-stu-id="77788-149">Get the list of all members in a chat.</span></span>|
|[<span data-ttu-id="77788-150">添加聊天成员</span><span class="sxs-lookup"><span data-stu-id="77788-150">Add chat member</span></span>](../api/chat-post-members.md) | <span data-ttu-id="77788-151">位置标头</span><span class="sxs-lookup"><span data-stu-id="77788-151">Location header</span></span> | <span data-ttu-id="77788-152">向聊天添加成员。</span><span class="sxs-lookup"><span data-stu-id="77788-152">Add a member to a chat.</span></span>| 
|[<span data-ttu-id="77788-153">获取聊天成员</span><span class="sxs-lookup"><span data-stu-id="77788-153">Get chat member</span></span>](../api/chat-get-members.md) | [<span data-ttu-id="77788-154">conversationMember</span><span class="sxs-lookup"><span data-stu-id="77788-154">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="77788-155">获取聊天中的成员。</span><span class="sxs-lookup"><span data-stu-id="77788-155">Get a member in a chat.</span></span>|
|[<span data-ttu-id="77788-156">删除聊天成员</span><span class="sxs-lookup"><span data-stu-id="77788-156">Remove chat member</span></span>](../api/chat-delete-members.md) | <span data-ttu-id="77788-157">Node</span><span class="sxs-lookup"><span data-stu-id="77788-157">Node</span></span> | <span data-ttu-id="77788-158">从聊天中删除成员。</span><span class="sxs-lookup"><span data-stu-id="77788-158">Remove a member from a chat.</span></span>| 

## <a name="properties"></a><span data-ttu-id="77788-159">属性</span><span class="sxs-lookup"><span data-stu-id="77788-159">Properties</span></span>

| <span data-ttu-id="77788-160">属性</span><span class="sxs-lookup"><span data-stu-id="77788-160">Property</span></span>   | <span data-ttu-id="77788-161">类型</span><span class="sxs-lookup"><span data-stu-id="77788-161">Type</span></span> |<span data-ttu-id="77788-162">说明</span><span class="sxs-lookup"><span data-stu-id="77788-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="77788-163">id</span><span class="sxs-lookup"><span data-stu-id="77788-163">id</span></span>|<span data-ttu-id="77788-164">String</span><span class="sxs-lookup"><span data-stu-id="77788-164">String</span></span>| <span data-ttu-id="77788-165">只读。</span><span class="sxs-lookup"><span data-stu-id="77788-165">Read-only.</span></span> <span data-ttu-id="77788-166">用户的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="77788-166">Unique ID of the user.</span></span>|
|<span data-ttu-id="77788-167">displayName</span><span class="sxs-lookup"><span data-stu-id="77788-167">displayName</span></span>| <span data-ttu-id="77788-168">string</span><span class="sxs-lookup"><span data-stu-id="77788-168">string</span></span> | <span data-ttu-id="77788-169">用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="77788-169">The display name of the user.</span></span> |
|<span data-ttu-id="77788-170">角色</span><span class="sxs-lookup"><span data-stu-id="77788-170">roles</span></span>| <span data-ttu-id="77788-171">string 集合</span><span class="sxs-lookup"><span data-stu-id="77788-171">string collection</span></span> | <span data-ttu-id="77788-172">该用户的角色。</span><span class="sxs-lookup"><span data-stu-id="77788-172">The roles for that user.</span></span> |
|<span data-ttu-id="77788-173">visibleHistoryStartDateTime</span><span class="sxs-lookup"><span data-stu-id="77788-173">visibleHistoryStartDateTime</span></span>| <span data-ttu-id="77788-174">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="77788-174">DateTimeOffset</span></span> | <span data-ttu-id="77788-175">表示对话历史记录与对话成员共享多远的时间戳。</span><span class="sxs-lookup"><span data-stu-id="77788-175">The timestamp denoting how far back a conversation's history is shared with the conversation member.</span></span> <span data-ttu-id="77788-176">此属性仅对聊天成员可设置。</span><span class="sxs-lookup"><span data-stu-id="77788-176">This property is settable only for members of a chat.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="77788-177">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="77788-177">JSON representation</span></span>

<span data-ttu-id="77788-178">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="77788-178">The following is a JSON representation of the resource.</span></span>

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


