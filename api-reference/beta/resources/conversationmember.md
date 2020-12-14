---
title: conversationMember 资源类型
description: 表示对话中的用户。
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2a8e4c94681065d9686e9f17888d3abf35885a65
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49658040"
---
# <a name="conversationmember-resource-type"></a><span data-ttu-id="eff36-103">conversationMember 资源类型</span><span class="sxs-lookup"><span data-stu-id="eff36-103">conversationMember resource type</span></span>

<span data-ttu-id="eff36-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eff36-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eff36-105">表示[聊天](chat.md)或[频道](channel.md)中的用户。</span><span class="sxs-lookup"><span data-stu-id="eff36-105">Represents a user in a [chat](chat.md) or a [channel](channel.md).</span></span>
<span data-ttu-id="eff36-106">另请参阅 [aadUserConversationMember](aaduserconversationmember.md)。</span><span class="sxs-lookup"><span data-stu-id="eff36-106">See also [aadUserConversationMember](aaduserconversationmember.md).</span></span>

## <a name="methods"></a><span data-ttu-id="eff36-107">方法</span><span class="sxs-lookup"><span data-stu-id="eff36-107">Methods</span></span>

| <span data-ttu-id="eff36-108">方法</span><span class="sxs-lookup"><span data-stu-id="eff36-108">Method</span></span>       | <span data-ttu-id="eff36-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="eff36-109">Return Type</span></span>  |<span data-ttu-id="eff36-110">说明</span><span class="sxs-lookup"><span data-stu-id="eff36-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="eff36-111">列出聊天成员</span><span class="sxs-lookup"><span data-stu-id="eff36-111">List chat members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="eff36-112">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="eff36-112">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="eff36-113">获取聊天中所有用户的列表。</span><span class="sxs-lookup"><span data-stu-id="eff36-113">Get the list of all users in the chat.</span></span>|
|[<span data-ttu-id="eff36-114">获取聊天成员</span><span class="sxs-lookup"><span data-stu-id="eff36-114">Get chat member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="eff36-115">conversationMember</span><span class="sxs-lookup"><span data-stu-id="eff36-115">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="eff36-116">获取聊天中的单个用户。</span><span class="sxs-lookup"><span data-stu-id="eff36-116">Get a single user in the chat.</span></span>|
|[<span data-ttu-id="eff36-117">列出团队成员</span><span class="sxs-lookup"><span data-stu-id="eff36-117">List team members</span></span>](../api/team-list-members.md)|<span data-ttu-id="eff36-118">[conversationMember](../resources/conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="eff36-118">[conversationMember](../resources/conversationmember.md) collection</span></span>|<span data-ttu-id="eff36-119">获取此团队中的成员列表。</span><span class="sxs-lookup"><span data-stu-id="eff36-119">Get the list of members in the team.</span></span>|
|[<span data-ttu-id="eff36-120">获取团队成员</span><span class="sxs-lookup"><span data-stu-id="eff36-120">Get team member</span></span>](../api/team-get-members.md) | <span data-ttu-id="eff36-121">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="eff36-121">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="eff36-122">获取团队中的成员。</span><span class="sxs-lookup"><span data-stu-id="eff36-122">Get a member in the team.</span></span>|
|[<span data-ttu-id="eff36-123">添加团队成员</span><span class="sxs-lookup"><span data-stu-id="eff36-123">Add team member</span></span>](../api/team-post-members.md)|[<span data-ttu-id="eff36-124">conversationMember</span><span class="sxs-lookup"><span data-stu-id="eff36-124">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="eff36-125">向团队中添加新成员。</span><span class="sxs-lookup"><span data-stu-id="eff36-125">Add a new member to the team.</span></span>|
|[<span data-ttu-id="eff36-126">批量添加团队成员</span><span class="sxs-lookup"><span data-stu-id="eff36-126">Add team members in bulk</span></span>](../api/conversationmembers-add.md)|<span data-ttu-id="eff36-127">[actionResultPart](../resources/actionresultpart.md) 集合</span><span class="sxs-lookup"><span data-stu-id="eff36-127">[actionResultPart](../resources/actionresultpart.md) collection</span></span>|<span data-ttu-id="eff36-128">在单个请求中向团队添加多个成员。</span><span class="sxs-lookup"><span data-stu-id="eff36-128">Add multiple members to the team in a single request.</span></span>|
|[<span data-ttu-id="eff36-129">更新团队成员的角色</span><span class="sxs-lookup"><span data-stu-id="eff36-129">Update team member's role</span></span>](../api/team-update-members.md)|[<span data-ttu-id="eff36-130">conversationMember</span><span class="sxs-lookup"><span data-stu-id="eff36-130">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="eff36-131">将成员更改为所有者或返回为常规成员。</span><span class="sxs-lookup"><span data-stu-id="eff36-131">Change a member to an owner or back to a regular member.</span></span>|
|[<span data-ttu-id="eff36-132">删除团队成员</span><span class="sxs-lookup"><span data-stu-id="eff36-132">Remove team member</span></span>](../api/team-delete-members.md)|<span data-ttu-id="eff36-133">无</span><span class="sxs-lookup"><span data-stu-id="eff36-133">None</span></span>|<span data-ttu-id="eff36-134">删除团队中的一个现有成员。</span><span class="sxs-lookup"><span data-stu-id="eff36-134">Remove an existing member from the team.</span></span>|
|[<span data-ttu-id="eff36-135">获取频道成员</span><span class="sxs-lookup"><span data-stu-id="eff36-135">Get channel member</span></span>](../api/channel-get-members.md) | <span data-ttu-id="eff36-136">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="eff36-136">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="eff36-137">获取频道中的成员。</span><span class="sxs-lookup"><span data-stu-id="eff36-137">Get a member in a channel.</span></span>|
|[<span data-ttu-id="eff36-138">创建频道成员</span><span class="sxs-lookup"><span data-stu-id="eff36-138">Create channel member</span></span>](../api/channel-post-members.md) | [<span data-ttu-id="eff36-139">conversationMember</span><span class="sxs-lookup"><span data-stu-id="eff36-139">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="eff36-140">向频道添加成员。</span><span class="sxs-lookup"><span data-stu-id="eff36-140">Add a member to a channel.</span></span> <span data-ttu-id="eff36-141">仅支持 membershipType 为 `private` 的 `channel`。</span><span class="sxs-lookup"><span data-stu-id="eff36-141">Only supported for `channel`with membershipType of `private`.</span></span>|
|[<span data-ttu-id="eff36-142">更新频道成员角色</span><span class="sxs-lookup"><span data-stu-id="eff36-142">Update channel member's role</span></span>](../api/channel-update-members.md) | [<span data-ttu-id="eff36-143">conversationMember</span><span class="sxs-lookup"><span data-stu-id="eff36-143">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="eff36-144">更新频道成员的属性。</span><span class="sxs-lookup"><span data-stu-id="eff36-144">Update the properties of a member of the channel.</span></span> <span data-ttu-id="eff36-145">仅支持 membershipType 为 `private` 的频道。</span><span class="sxs-lookup"><span data-stu-id="eff36-145">Only supported for channel with membershipType of `private`.</span></span>|
|[<span data-ttu-id="eff36-146">删除频道成员</span><span class="sxs-lookup"><span data-stu-id="eff36-146">Remove channel member</span></span>](../api/channel-delete-members.md) | <span data-ttu-id="eff36-147">无</span><span class="sxs-lookup"><span data-stu-id="eff36-147">None</span></span> | <span data-ttu-id="eff36-148">从频道中删除一个成员。</span><span class="sxs-lookup"><span data-stu-id="eff36-148">Delete a member from a channel.</span></span> <span data-ttu-id="eff36-149">仅支持用于 `private` 的 `channelType`。</span><span class="sxs-lookup"><span data-stu-id="eff36-149">Only supported for `channelType` of `private`.</span></span>|



## <a name="properties"></a><span data-ttu-id="eff36-150">属性</span><span class="sxs-lookup"><span data-stu-id="eff36-150">Properties</span></span>

| <span data-ttu-id="eff36-151">属性</span><span class="sxs-lookup"><span data-stu-id="eff36-151">Property</span></span>   | <span data-ttu-id="eff36-152">类型</span><span class="sxs-lookup"><span data-stu-id="eff36-152">Type</span></span> |<span data-ttu-id="eff36-153">说明</span><span class="sxs-lookup"><span data-stu-id="eff36-153">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eff36-154">id</span><span class="sxs-lookup"><span data-stu-id="eff36-154">id</span></span>|<span data-ttu-id="eff36-155">String</span><span class="sxs-lookup"><span data-stu-id="eff36-155">String</span></span>| <span data-ttu-id="eff36-156">只读。</span><span class="sxs-lookup"><span data-stu-id="eff36-156">Read-only.</span></span> <span data-ttu-id="eff36-157">用户的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="eff36-157">Unique ID of the user.</span></span>|
|<span data-ttu-id="eff36-158">displayName</span><span class="sxs-lookup"><span data-stu-id="eff36-158">displayName</span></span>| <span data-ttu-id="eff36-159">string</span><span class="sxs-lookup"><span data-stu-id="eff36-159">string</span></span> | <span data-ttu-id="eff36-160">用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="eff36-160">The display name of the user.</span></span> |
|<span data-ttu-id="eff36-161">角色</span><span class="sxs-lookup"><span data-stu-id="eff36-161">roles</span></span>| <span data-ttu-id="eff36-162">string 集合</span><span class="sxs-lookup"><span data-stu-id="eff36-162">string collection</span></span> | <span data-ttu-id="eff36-163">该用户的角色。</span><span class="sxs-lookup"><span data-stu-id="eff36-163">The roles for that user.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="eff36-164">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="eff36-164">JSON representation</span></span>

<span data-ttu-id="eff36-165">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eff36-165">The following is a JSON representation of the resource.</span></span>

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


