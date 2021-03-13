---
title: conversationMember 资源类型
description: 表示对话中的用户。
localization_priority: Normal
author: laujan
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 14a70fcc6492ec143fa2f4e892438805d3526d60
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777718"
---
# <a name="conversationmember-resource-type"></a><span data-ttu-id="41394-103">conversationMember 资源类型</span><span class="sxs-lookup"><span data-stu-id="41394-103">conversationMember resource type</span></span>

<span data-ttu-id="41394-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41394-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="41394-105">表示[团队、频道](team.md)[或](channel.md)聊天中的[用户](chat.md)。</span><span class="sxs-lookup"><span data-stu-id="41394-105">Represents a user in a [team](team.md), a [channel](channel.md), or a [chat](chat.md).</span></span>
<span data-ttu-id="41394-106">另请参阅 [aadUserConversationMember](aaduserconversationmember.md)。</span><span class="sxs-lookup"><span data-stu-id="41394-106">See also [aadUserConversationMember](aaduserconversationmember.md).</span></span>

## <a name="methods"></a><span data-ttu-id="41394-107">方法</span><span class="sxs-lookup"><span data-stu-id="41394-107">Methods</span></span>

| <span data-ttu-id="41394-108">方法</span><span class="sxs-lookup"><span data-stu-id="41394-108">Method</span></span>       | <span data-ttu-id="41394-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="41394-109">Return Type</span></span>  |<span data-ttu-id="41394-110">说明</span><span class="sxs-lookup"><span data-stu-id="41394-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="41394-111">列出团队成员</span><span class="sxs-lookup"><span data-stu-id="41394-111">List team members</span></span>](../api/team-list-members.md)|<span data-ttu-id="41394-112">[conversationMember](../resources/conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="41394-112">[conversationMember](../resources/conversationmember.md) collection</span></span>|<span data-ttu-id="41394-113">获取此团队中的成员列表。</span><span class="sxs-lookup"><span data-stu-id="41394-113">Get the list of members in the team.</span></span>|
|[<span data-ttu-id="41394-114">添加团队成员</span><span class="sxs-lookup"><span data-stu-id="41394-114">Add team member</span></span>](../api/team-post-members.md)|[<span data-ttu-id="41394-115">conversationMember</span><span class="sxs-lookup"><span data-stu-id="41394-115">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="41394-116">向团队中添加新成员。</span><span class="sxs-lookup"><span data-stu-id="41394-116">Add a new member to the team.</span></span>|
|[<span data-ttu-id="41394-117">获取团队成员</span><span class="sxs-lookup"><span data-stu-id="41394-117">Get team member</span></span>](../api/team-get-members.md) | <span data-ttu-id="41394-118">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="41394-118">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="41394-119">获取团队中的成员。</span><span class="sxs-lookup"><span data-stu-id="41394-119">Get a member in the team.</span></span>|
|[<span data-ttu-id="41394-120">更新成员角色</span><span class="sxs-lookup"><span data-stu-id="41394-120">Update team member's role</span></span>](../api/team-update-members.md)|[<span data-ttu-id="41394-121">conversationMember</span><span class="sxs-lookup"><span data-stu-id="41394-121">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="41394-122">将成员更改为所有者或返回为常规成员。</span><span class="sxs-lookup"><span data-stu-id="41394-122">Change a member to an owner or back to a regular member.</span></span>|
|[<span data-ttu-id="41394-123">删除团队成员</span><span class="sxs-lookup"><span data-stu-id="41394-123">Remove team member</span></span>](../api/team-delete-members.md)|<span data-ttu-id="41394-124">无</span><span class="sxs-lookup"><span data-stu-id="41394-124">None</span></span>|<span data-ttu-id="41394-125">删除团队中的一个现有成员。</span><span class="sxs-lookup"><span data-stu-id="41394-125">Remove an existing member from the team.</span></span>|
|[<span data-ttu-id="41394-126">列出频道成员</span><span class="sxs-lookup"><span data-stu-id="41394-126">List channel members</span></span>](../api/channel-list-members.md) | <span data-ttu-id="41394-127">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="41394-127">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="41394-128">获取频道中的所有成员列表。</span><span class="sxs-lookup"><span data-stu-id="41394-128">Get the list of all members in a channel.</span></span>|
|[<span data-ttu-id="41394-129">添加频道成员</span><span class="sxs-lookup"><span data-stu-id="41394-129">Add channel member</span></span>](../api/channel-post-members.md) | [<span data-ttu-id="41394-130">conversationMember</span><span class="sxs-lookup"><span data-stu-id="41394-130">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="41394-131">向频道添加成员。</span><span class="sxs-lookup"><span data-stu-id="41394-131">Add a member to a channel.</span></span> <span data-ttu-id="41394-132">仅支持 membershipType 为 `private` 的 `channel`。</span><span class="sxs-lookup"><span data-stu-id="41394-132">Only supported for `channel` with membershipType of `private`.</span></span>|
|[<span data-ttu-id="41394-133">获取频道成员</span><span class="sxs-lookup"><span data-stu-id="41394-133">Get channel member</span></span>](../api/channel-get-members.md) | <span data-ttu-id="41394-134">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="41394-134">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="41394-135">获取频道中的成员。</span><span class="sxs-lookup"><span data-stu-id="41394-135">Get a member in a channel.</span></span>|
|[<span data-ttu-id="41394-136">更新频道成员角色</span><span class="sxs-lookup"><span data-stu-id="41394-136">Update channel member's role</span></span>](../api/channel-update-members.md) | [<span data-ttu-id="41394-137">conversationMember</span><span class="sxs-lookup"><span data-stu-id="41394-137">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="41394-138">更新频道成员的属性。</span><span class="sxs-lookup"><span data-stu-id="41394-138">Update the properties of a member of the channel.</span></span> <span data-ttu-id="41394-139">仅支持 membershipType 为 `private` 的频道。</span><span class="sxs-lookup"><span data-stu-id="41394-139">Only supported for channel with membershipType of `private`.</span></span>|
|[<span data-ttu-id="41394-140">删除频道成员</span><span class="sxs-lookup"><span data-stu-id="41394-140">Remove channel member</span></span>](../api/channel-delete-members.md) | <span data-ttu-id="41394-141">无</span><span class="sxs-lookup"><span data-stu-id="41394-141">None</span></span> | <span data-ttu-id="41394-142">从频道中删除一个成员。</span><span class="sxs-lookup"><span data-stu-id="41394-142">Delete a member from a channel.</span></span> <span data-ttu-id="41394-143">仅支持用于 `private` 的 `channelType`。</span><span class="sxs-lookup"><span data-stu-id="41394-143">Only supported for `channelType` of `private`.</span></span>|
|[<span data-ttu-id="41394-144">列出聊天成员</span><span class="sxs-lookup"><span data-stu-id="41394-144">List chat members</span></span>](../api/chat-list-members.md) | <span data-ttu-id="41394-145">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="41394-145">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="41394-146">获取聊天中的所有成员列表。</span><span class="sxs-lookup"><span data-stu-id="41394-146">Get the list of all members in a chat.</span></span>|
|[<span data-ttu-id="41394-147">添加聊天成员</span><span class="sxs-lookup"><span data-stu-id="41394-147">Add chat member</span></span>](../api/chat-post-members.md) | <span data-ttu-id="41394-148">位置标头</span><span class="sxs-lookup"><span data-stu-id="41394-148">Location header</span></span> | <span data-ttu-id="41394-149">向聊天添加成员。</span><span class="sxs-lookup"><span data-stu-id="41394-149">Add a member to a chat.</span></span>| 
|[<span data-ttu-id="41394-150">获取聊天成员</span><span class="sxs-lookup"><span data-stu-id="41394-150">Get chat member</span></span>](../api/chat-get-members.md) | [<span data-ttu-id="41394-151">conversationMember</span><span class="sxs-lookup"><span data-stu-id="41394-151">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="41394-152">获取聊天中的成员。</span><span class="sxs-lookup"><span data-stu-id="41394-152">Get a member in a chat.</span></span>|
|[<span data-ttu-id="41394-153">删除聊天成员</span><span class="sxs-lookup"><span data-stu-id="41394-153">Remove chat member</span></span>](../api/chat-delete-members.md) | <span data-ttu-id="41394-154">无</span><span class="sxs-lookup"><span data-stu-id="41394-154">None</span></span> | <span data-ttu-id="41394-155">从聊天中删除成员。</span><span class="sxs-lookup"><span data-stu-id="41394-155">Remove a member from a chat.</span></span>| 

## <a name="properties"></a><span data-ttu-id="41394-156">属性</span><span class="sxs-lookup"><span data-stu-id="41394-156">Properties</span></span>

| <span data-ttu-id="41394-157">属性</span><span class="sxs-lookup"><span data-stu-id="41394-157">Property</span></span>   | <span data-ttu-id="41394-158">类型</span><span class="sxs-lookup"><span data-stu-id="41394-158">Type</span></span> |<span data-ttu-id="41394-159">说明</span><span class="sxs-lookup"><span data-stu-id="41394-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="41394-160">id</span><span class="sxs-lookup"><span data-stu-id="41394-160">id</span></span>|<span data-ttu-id="41394-161">字符串</span><span class="sxs-lookup"><span data-stu-id="41394-161">String</span></span>| <span data-ttu-id="41394-162">只读。</span><span class="sxs-lookup"><span data-stu-id="41394-162">Read-only.</span></span> <span data-ttu-id="41394-163">用户的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="41394-163">Unique ID of the user.</span></span>|
|<span data-ttu-id="41394-164">displayName</span><span class="sxs-lookup"><span data-stu-id="41394-164">displayName</span></span>| <span data-ttu-id="41394-165">string</span><span class="sxs-lookup"><span data-stu-id="41394-165">string</span></span> | <span data-ttu-id="41394-166">用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="41394-166">The display name of the user.</span></span> |
|<span data-ttu-id="41394-167">角色</span><span class="sxs-lookup"><span data-stu-id="41394-167">roles</span></span>| <span data-ttu-id="41394-168">string 集合</span><span class="sxs-lookup"><span data-stu-id="41394-168">string collection</span></span> | <span data-ttu-id="41394-169">该用户的角色。</span><span class="sxs-lookup"><span data-stu-id="41394-169">The roles for that user.</span></span> |
|<span data-ttu-id="41394-170">visibleHistoryStartDateTime</span><span class="sxs-lookup"><span data-stu-id="41394-170">visibleHistoryStartDateTime</span></span>| <span data-ttu-id="41394-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="41394-171">DateTimeOffset</span></span> | <span data-ttu-id="41394-172">表示对话历史久远程度的时间戳与对话成员共享。</span><span class="sxs-lookup"><span data-stu-id="41394-172">The timestamp denoting how far back a conversation's history is shared with the conversation member.</span></span> <span data-ttu-id="41394-173">此属性只对聊天成员可设置。</span><span class="sxs-lookup"><span data-stu-id="41394-173">This property is settable only for members of a chat.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="41394-174">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="41394-174">JSON representation</span></span>

<span data-ttu-id="41394-175">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="41394-175">The following is a JSON representation of the resource.</span></span>

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

