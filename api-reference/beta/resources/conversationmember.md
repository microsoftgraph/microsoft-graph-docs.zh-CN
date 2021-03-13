---
title: conversationMember 资源类型
description: 表示对话中的用户。
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: caa084ecb1d1d468e9be237f22bed2ab80cd1b41
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772413"
---
# <a name="conversationmember-resource-type"></a><span data-ttu-id="9a060-103">conversationMember 资源类型</span><span class="sxs-lookup"><span data-stu-id="9a060-103">conversationMember resource type</span></span>

<span data-ttu-id="9a060-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a060-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a060-105">表示团队、 [频道](team.md) 或 [聊天](channel.md) 中的 [用户](chat.md)。</span><span class="sxs-lookup"><span data-stu-id="9a060-105">Represents a user in a [team](team.md) or a [channel](channel.md) or a [chat](chat.md).</span></span>
<span data-ttu-id="9a060-106">另请参阅 [aadUserConversationMember](aaduserconversationmember.md)。</span><span class="sxs-lookup"><span data-stu-id="9a060-106">See also [aadUserConversationMember](aaduserconversationmember.md).</span></span>

## <a name="methods"></a><span data-ttu-id="9a060-107">方法</span><span class="sxs-lookup"><span data-stu-id="9a060-107">Methods</span></span>

| <span data-ttu-id="9a060-108">方法</span><span class="sxs-lookup"><span data-stu-id="9a060-108">Method</span></span>       | <span data-ttu-id="9a060-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="9a060-109">Return Type</span></span>  |<span data-ttu-id="9a060-110">说明</span><span class="sxs-lookup"><span data-stu-id="9a060-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9a060-111">列出团队成员</span><span class="sxs-lookup"><span data-stu-id="9a060-111">List team members</span></span>](../api/team-list-members.md)|<span data-ttu-id="9a060-112">[conversationMember](../resources/conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9a060-112">[conversationMember](../resources/conversationmember.md) collection</span></span>|<span data-ttu-id="9a060-113">获取此团队中的成员列表。</span><span class="sxs-lookup"><span data-stu-id="9a060-113">Get the list of members in the team.</span></span>|
|[<span data-ttu-id="9a060-114">添加团队成员</span><span class="sxs-lookup"><span data-stu-id="9a060-114">Add team member</span></span>](../api/team-post-members.md)|[<span data-ttu-id="9a060-115">conversationMember</span><span class="sxs-lookup"><span data-stu-id="9a060-115">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="9a060-116">向团队中添加新成员。</span><span class="sxs-lookup"><span data-stu-id="9a060-116">Add a new member to the team.</span></span>|
|[<span data-ttu-id="9a060-117">批量添加团队成员。</span><span class="sxs-lookup"><span data-stu-id="9a060-117">Add team members in bulk</span></span>](../api/conversationmembers-add.md)|<span data-ttu-id="9a060-118">[actionResultPart](../resources/actionresultpart.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9a060-118">[actionResultPart](../resources/actionresultpart.md) collection</span></span>|<span data-ttu-id="9a060-119">在单个请求中将多个成员添加到团队中。</span><span class="sxs-lookup"><span data-stu-id="9a060-119">Add multiple members to the team in a single request.</span></span>|
|[<span data-ttu-id="9a060-120">获取团队成员</span><span class="sxs-lookup"><span data-stu-id="9a060-120">Get team member</span></span>](../api/team-get-members.md) | <span data-ttu-id="9a060-121">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9a060-121">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="9a060-122">获取团队中的成员。</span><span class="sxs-lookup"><span data-stu-id="9a060-122">Get a member in the team.</span></span>|
|[<span data-ttu-id="9a060-123">更新成员角色</span><span class="sxs-lookup"><span data-stu-id="9a060-123">Update team member's role</span></span>](../api/team-update-members.md)|[<span data-ttu-id="9a060-124">conversationMember</span><span class="sxs-lookup"><span data-stu-id="9a060-124">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="9a060-125">将成员更改为所有者或返回为常规成员。</span><span class="sxs-lookup"><span data-stu-id="9a060-125">Change a member to an owner or back to a regular member.</span></span>|
|[<span data-ttu-id="9a060-126">删除团队成员</span><span class="sxs-lookup"><span data-stu-id="9a060-126">Remove team member</span></span>](../api/team-delete-members.md)|<span data-ttu-id="9a060-127">无</span><span class="sxs-lookup"><span data-stu-id="9a060-127">None</span></span>|<span data-ttu-id="9a060-128">删除团队中的一个现有成员。</span><span class="sxs-lookup"><span data-stu-id="9a060-128">Remove an existing member from the team.</span></span>|
|[<span data-ttu-id="9a060-129">列出频道成员</span><span class="sxs-lookup"><span data-stu-id="9a060-129">List channel members</span></span>](../api/channel-list-members.md) | <span data-ttu-id="9a060-130">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9a060-130">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="9a060-131">获取频道中的所有成员列表。</span><span class="sxs-lookup"><span data-stu-id="9a060-131">Get the list of all members in a channel.</span></span>|
|[<span data-ttu-id="9a060-132">添加频道成员</span><span class="sxs-lookup"><span data-stu-id="9a060-132">Add channel member</span></span>](../api/channel-post-members.md) | [<span data-ttu-id="9a060-133">conversationMember</span><span class="sxs-lookup"><span data-stu-id="9a060-133">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="9a060-134">向频道添加成员。</span><span class="sxs-lookup"><span data-stu-id="9a060-134">Add a member to a channel.</span></span> <span data-ttu-id="9a060-135">仅支持 membershipType 为 `private` 的 `channel`。</span><span class="sxs-lookup"><span data-stu-id="9a060-135">Only supported for `channel` with membershipType of `private`.</span></span>|
|[<span data-ttu-id="9a060-136">获取频道成员</span><span class="sxs-lookup"><span data-stu-id="9a060-136">Get channel member</span></span>](../api/channel-get-members.md) | <span data-ttu-id="9a060-137">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9a060-137">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="9a060-138">获取频道中的成员。</span><span class="sxs-lookup"><span data-stu-id="9a060-138">Get a member in a channel.</span></span>|
|[<span data-ttu-id="9a060-139">更新频道成员角色</span><span class="sxs-lookup"><span data-stu-id="9a060-139">Update channel member's role</span></span>](../api/channel-update-members.md) | [<span data-ttu-id="9a060-140">conversationMember</span><span class="sxs-lookup"><span data-stu-id="9a060-140">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="9a060-141">更新频道成员的属性。</span><span class="sxs-lookup"><span data-stu-id="9a060-141">Update the properties of a member of the channel.</span></span> <span data-ttu-id="9a060-142">仅支持 membershipType 为 `private` 的频道。</span><span class="sxs-lookup"><span data-stu-id="9a060-142">Only supported for channel with membershipType of `private`.</span></span>|
|[<span data-ttu-id="9a060-143">删除频道成员</span><span class="sxs-lookup"><span data-stu-id="9a060-143">Remove channel member</span></span>](../api/channel-delete-members.md) | <span data-ttu-id="9a060-144">无</span><span class="sxs-lookup"><span data-stu-id="9a060-144">None</span></span> | <span data-ttu-id="9a060-145">从频道中删除一个成员。</span><span class="sxs-lookup"><span data-stu-id="9a060-145">Delete a member from a channel.</span></span> <span data-ttu-id="9a060-146">仅支持用于 `private` 的 `channelType`。</span><span class="sxs-lookup"><span data-stu-id="9a060-146">Only supported for `channelType` of `private`.</span></span>|
|[<span data-ttu-id="9a060-147">列出聊天成员</span><span class="sxs-lookup"><span data-stu-id="9a060-147">List chat members</span></span>](../api/chat-list-members.md) | <span data-ttu-id="9a060-148">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9a060-148">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="9a060-149">获取聊天中的所有成员列表。</span><span class="sxs-lookup"><span data-stu-id="9a060-149">Get the list of all members in a chat.</span></span>|
|[<span data-ttu-id="9a060-150">添加聊天成员</span><span class="sxs-lookup"><span data-stu-id="9a060-150">Add chat member</span></span>](../api/chat-post-members.md) | <span data-ttu-id="9a060-151">位置标头</span><span class="sxs-lookup"><span data-stu-id="9a060-151">Location header</span></span> | <span data-ttu-id="9a060-152">向聊天添加成员。</span><span class="sxs-lookup"><span data-stu-id="9a060-152">Add a member to a chat.</span></span>| 
|[<span data-ttu-id="9a060-153">获取聊天成员</span><span class="sxs-lookup"><span data-stu-id="9a060-153">Get chat member</span></span>](../api/chat-get-members.md) | [<span data-ttu-id="9a060-154">conversationMember</span><span class="sxs-lookup"><span data-stu-id="9a060-154">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="9a060-155">获取聊天中的成员。</span><span class="sxs-lookup"><span data-stu-id="9a060-155">Get a member in a chat.</span></span>|
|[<span data-ttu-id="9a060-156">删除聊天成员</span><span class="sxs-lookup"><span data-stu-id="9a060-156">Remove chat member</span></span>](../api/chat-delete-members.md) | <span data-ttu-id="9a060-157">无</span><span class="sxs-lookup"><span data-stu-id="9a060-157">None</span></span> | <span data-ttu-id="9a060-158">从聊天中删除成员。</span><span class="sxs-lookup"><span data-stu-id="9a060-158">Remove a member from a chat.</span></span>| 

## <a name="properties"></a><span data-ttu-id="9a060-159">属性</span><span class="sxs-lookup"><span data-stu-id="9a060-159">Properties</span></span>

| <span data-ttu-id="9a060-160">属性</span><span class="sxs-lookup"><span data-stu-id="9a060-160">Property</span></span>   | <span data-ttu-id="9a060-161">类型</span><span class="sxs-lookup"><span data-stu-id="9a060-161">Type</span></span> |<span data-ttu-id="9a060-162">说明</span><span class="sxs-lookup"><span data-stu-id="9a060-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9a060-163">id</span><span class="sxs-lookup"><span data-stu-id="9a060-163">id</span></span>|<span data-ttu-id="9a060-164">字符串</span><span class="sxs-lookup"><span data-stu-id="9a060-164">String</span></span>| <span data-ttu-id="9a060-165">只读。</span><span class="sxs-lookup"><span data-stu-id="9a060-165">Read-only.</span></span> <span data-ttu-id="9a060-166">用户的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="9a060-166">Unique ID of the user.</span></span>|
|<span data-ttu-id="9a060-167">displayName</span><span class="sxs-lookup"><span data-stu-id="9a060-167">displayName</span></span>| <span data-ttu-id="9a060-168">string</span><span class="sxs-lookup"><span data-stu-id="9a060-168">string</span></span> | <span data-ttu-id="9a060-169">用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="9a060-169">The display name of the user.</span></span> |
|<span data-ttu-id="9a060-170">角色</span><span class="sxs-lookup"><span data-stu-id="9a060-170">roles</span></span>| <span data-ttu-id="9a060-171">string 集合</span><span class="sxs-lookup"><span data-stu-id="9a060-171">string collection</span></span> | <span data-ttu-id="9a060-172">该用户的角色。</span><span class="sxs-lookup"><span data-stu-id="9a060-172">The roles for that user.</span></span> |
|<span data-ttu-id="9a060-173">visibleHistoryStartDateTime</span><span class="sxs-lookup"><span data-stu-id="9a060-173">visibleHistoryStartDateTime</span></span>| <span data-ttu-id="9a060-174">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9a060-174">DateTimeOffset</span></span> | <span data-ttu-id="9a060-175">表示对话历史久远程度的时间戳与对话成员共享。</span><span class="sxs-lookup"><span data-stu-id="9a060-175">The timestamp denoting how far back a conversation's history is shared with the conversation member.</span></span> <span data-ttu-id="9a060-176">此属性只对聊天成员可设置。</span><span class="sxs-lookup"><span data-stu-id="9a060-176">This property is settable only for members of a chat.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9a060-177">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9a060-177">JSON representation</span></span>

<span data-ttu-id="9a060-178">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9a060-178">The following is a JSON representation of the resource.</span></span>

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


