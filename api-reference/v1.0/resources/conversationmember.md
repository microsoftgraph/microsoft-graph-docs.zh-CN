---
title: conversationMember 资源类型
description: 代表对话中的用户。
localization_priority: Normal
author: laujan
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2d2e44349f7896dfed0d0dff455e9afd0ac65772
ms.sourcegitcommit: 0d4377b0153bc339ab7b3b1a6ee4d52848b622d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2020
ms.locfileid: "49714275"
---
# <a name="conversationmember-resource-type"></a><span data-ttu-id="a4612-103">conversationMember 资源类型</span><span class="sxs-lookup"><span data-stu-id="a4612-103">conversationMember resource type</span></span>

<span data-ttu-id="a4612-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4612-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a4612-105">表示[团队、频道](team.md)[或聊天](channel.md)中的[用户](chat.md)。</span><span class="sxs-lookup"><span data-stu-id="a4612-105">Represents a user in a [team](team.md), a [channel](channel.md), or a [chat](chat.md).</span></span>
<span data-ttu-id="a4612-106">另请参阅 [aadUserConversationMember](aaduserconversationmember.md)。</span><span class="sxs-lookup"><span data-stu-id="a4612-106">See also [aadUserConversationMember](aaduserconversationmember.md).</span></span>

## <a name="methods"></a><span data-ttu-id="a4612-107">方法</span><span class="sxs-lookup"><span data-stu-id="a4612-107">Methods</span></span>

| <span data-ttu-id="a4612-108">方法</span><span class="sxs-lookup"><span data-stu-id="a4612-108">Method</span></span>       | <span data-ttu-id="a4612-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="a4612-109">Return Type</span></span>  |<span data-ttu-id="a4612-110">说明</span><span class="sxs-lookup"><span data-stu-id="a4612-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a4612-111">列出团队成员</span><span class="sxs-lookup"><span data-stu-id="a4612-111">List team members</span></span>](../api/team-list-members.md)|<span data-ttu-id="a4612-112">[conversationMember](../resources/conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a4612-112">[conversationMember](../resources/conversationmember.md) collection</span></span>|<span data-ttu-id="a4612-113">获取此团队中的成员列表。</span><span class="sxs-lookup"><span data-stu-id="a4612-113">Get the list of members in the team.</span></span>|
|[<span data-ttu-id="a4612-114">添加团队成员</span><span class="sxs-lookup"><span data-stu-id="a4612-114">Add team member</span></span>](../api/team-post-members.md)|[<span data-ttu-id="a4612-115">conversationMember</span><span class="sxs-lookup"><span data-stu-id="a4612-115">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="a4612-116">向团队中添加新成员。</span><span class="sxs-lookup"><span data-stu-id="a4612-116">Add a new member to the team.</span></span>|
|[<span data-ttu-id="a4612-117">获取团队成员</span><span class="sxs-lookup"><span data-stu-id="a4612-117">Get team member</span></span>](../api/team-get-members.md) | <span data-ttu-id="a4612-118">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a4612-118">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="a4612-119">获取团队中的成员。</span><span class="sxs-lookup"><span data-stu-id="a4612-119">Get a member in the team.</span></span>|
|[<span data-ttu-id="a4612-120">更新成员角色</span><span class="sxs-lookup"><span data-stu-id="a4612-120">Update team member's role</span></span>](../api/team-update-members.md)|[<span data-ttu-id="a4612-121">conversationMember</span><span class="sxs-lookup"><span data-stu-id="a4612-121">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="a4612-122">将成员更改为所有者或返回为常规成员。</span><span class="sxs-lookup"><span data-stu-id="a4612-122">Change a member to an owner or back to a regular member.</span></span>|
|[<span data-ttu-id="a4612-123">删除团队成员</span><span class="sxs-lookup"><span data-stu-id="a4612-123">Remove team member</span></span>](../api/team-delete-members.md)|<span data-ttu-id="a4612-124">无</span><span class="sxs-lookup"><span data-stu-id="a4612-124">None</span></span>|<span data-ttu-id="a4612-125">删除团队中的一个现有成员。</span><span class="sxs-lookup"><span data-stu-id="a4612-125">Remove an existing member from the team.</span></span>|
|[<span data-ttu-id="a4612-126">列出频道成员</span><span class="sxs-lookup"><span data-stu-id="a4612-126">List channel members</span></span>](../api/channel-list-members.md) | <span data-ttu-id="a4612-127">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a4612-127">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="a4612-128">获取频道中的所有成员列表。</span><span class="sxs-lookup"><span data-stu-id="a4612-128">Get the list of all members in a channel.</span></span>|
|[<span data-ttu-id="a4612-129">添加频道成员</span><span class="sxs-lookup"><span data-stu-id="a4612-129">Add channel member</span></span>](../api/channel-post-members.md) | [<span data-ttu-id="a4612-130">conversationMember</span><span class="sxs-lookup"><span data-stu-id="a4612-130">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="a4612-131">向频道添加成员。</span><span class="sxs-lookup"><span data-stu-id="a4612-131">Add a member to a channel.</span></span> <span data-ttu-id="a4612-132">仅支持 membershipType 为 `private` 的 `channel`。</span><span class="sxs-lookup"><span data-stu-id="a4612-132">Only supported for `channel`with membershipType of `private`.</span></span>|
|[<span data-ttu-id="a4612-133">获取频道成员</span><span class="sxs-lookup"><span data-stu-id="a4612-133">Get channel member</span></span>](../api/channel-get-members.md) | <span data-ttu-id="a4612-134">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a4612-134">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="a4612-135">获取频道中的成员。</span><span class="sxs-lookup"><span data-stu-id="a4612-135">Get a member in a channel.</span></span>|
|[<span data-ttu-id="a4612-136">更新频道成员角色</span><span class="sxs-lookup"><span data-stu-id="a4612-136">Update channel member's role</span></span>](../api/channel-update-members.md) | [<span data-ttu-id="a4612-137">conversationMember</span><span class="sxs-lookup"><span data-stu-id="a4612-137">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="a4612-138">更新频道成员的属性。</span><span class="sxs-lookup"><span data-stu-id="a4612-138">Update the properties of a member of the channel.</span></span> <span data-ttu-id="a4612-139">仅支持 membershipType 为 `private` 的频道。</span><span class="sxs-lookup"><span data-stu-id="a4612-139">Only supported for channel with membershipType of `private`.</span></span>|
|[<span data-ttu-id="a4612-140">删除频道成员</span><span class="sxs-lookup"><span data-stu-id="a4612-140">Remove channel member</span></span>](../api/channel-delete-members.md) | <span data-ttu-id="a4612-141">无</span><span class="sxs-lookup"><span data-stu-id="a4612-141">None</span></span> | <span data-ttu-id="a4612-142">从频道中删除一个成员。</span><span class="sxs-lookup"><span data-stu-id="a4612-142">Delete a member from a channel.</span></span> <span data-ttu-id="a4612-143">仅支持用于 `private` 的 `channelType`。</span><span class="sxs-lookup"><span data-stu-id="a4612-143">Only supported for `channelType` of `private`.</span></span>|

## <a name="properties"></a><span data-ttu-id="a4612-144">属性</span><span class="sxs-lookup"><span data-stu-id="a4612-144">Properties</span></span>

| <span data-ttu-id="a4612-145">属性</span><span class="sxs-lookup"><span data-stu-id="a4612-145">Property</span></span>   | <span data-ttu-id="a4612-146">类型</span><span class="sxs-lookup"><span data-stu-id="a4612-146">Type</span></span> |<span data-ttu-id="a4612-147">说明</span><span class="sxs-lookup"><span data-stu-id="a4612-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a4612-148">id</span><span class="sxs-lookup"><span data-stu-id="a4612-148">id</span></span>|<span data-ttu-id="a4612-149">String</span><span class="sxs-lookup"><span data-stu-id="a4612-149">String</span></span>| <span data-ttu-id="a4612-150">只读。</span><span class="sxs-lookup"><span data-stu-id="a4612-150">Read-only.</span></span> <span data-ttu-id="a4612-151">用户的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="a4612-151">Unique ID of the user.</span></span>|
|<span data-ttu-id="a4612-152">displayName</span><span class="sxs-lookup"><span data-stu-id="a4612-152">displayName</span></span>| <span data-ttu-id="a4612-153">string</span><span class="sxs-lookup"><span data-stu-id="a4612-153">string</span></span> | <span data-ttu-id="a4612-154">用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="a4612-154">The display name of the user.</span></span> |
|<span data-ttu-id="a4612-155">角色</span><span class="sxs-lookup"><span data-stu-id="a4612-155">roles</span></span>| <span data-ttu-id="a4612-156">string 集合</span><span class="sxs-lookup"><span data-stu-id="a4612-156">string collection</span></span> | <span data-ttu-id="a4612-157">该用户的角色。</span><span class="sxs-lookup"><span data-stu-id="a4612-157">The roles for that user.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a4612-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a4612-158">JSON representation</span></span>

<span data-ttu-id="a4612-159">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a4612-159">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.conversationMember",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "displayName": "String",
  "id": "String (identifier)",
  "roles": ["String"]
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

