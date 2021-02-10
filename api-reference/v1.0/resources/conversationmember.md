---
title: conversationMember 资源类型
description: 表示对话中的用户。
localization_priority: Normal
author: laujan
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 1629b46b12d91fd96dca72577027f0031ab0102a
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161787"
---
# <a name="conversationmember-resource-type"></a><span data-ttu-id="a81b1-103">conversationMember 资源类型</span><span class="sxs-lookup"><span data-stu-id="a81b1-103">conversationMember resource type</span></span>

<span data-ttu-id="a81b1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a81b1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a81b1-105">表示团队[、](team.md)[频道或聊天](channel.md)中的[用户](chat.md)。</span><span class="sxs-lookup"><span data-stu-id="a81b1-105">Represents a user in a [team](team.md), a [channel](channel.md), or a [chat](chat.md).</span></span>
<span data-ttu-id="a81b1-106">另请参阅 [aadUserConversationMember](aaduserconversationmember.md)。</span><span class="sxs-lookup"><span data-stu-id="a81b1-106">See also [aadUserConversationMember](aaduserconversationmember.md).</span></span>

## <a name="methods"></a><span data-ttu-id="a81b1-107">方法</span><span class="sxs-lookup"><span data-stu-id="a81b1-107">Methods</span></span>

| <span data-ttu-id="a81b1-108">方法</span><span class="sxs-lookup"><span data-stu-id="a81b1-108">Method</span></span>       | <span data-ttu-id="a81b1-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="a81b1-109">Return Type</span></span>  |<span data-ttu-id="a81b1-110">说明</span><span class="sxs-lookup"><span data-stu-id="a81b1-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a81b1-111">列出团队成员</span><span class="sxs-lookup"><span data-stu-id="a81b1-111">List team members</span></span>](../api/team-list-members.md)|<span data-ttu-id="a81b1-112">[conversationMember](../resources/conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a81b1-112">[conversationMember](../resources/conversationmember.md) collection</span></span>|<span data-ttu-id="a81b1-113">获取此团队中的成员列表。</span><span class="sxs-lookup"><span data-stu-id="a81b1-113">Get the list of members in the team.</span></span>|
|[<span data-ttu-id="a81b1-114">添加团队成员</span><span class="sxs-lookup"><span data-stu-id="a81b1-114">Add team member</span></span>](../api/team-post-members.md)|[<span data-ttu-id="a81b1-115">conversationMember</span><span class="sxs-lookup"><span data-stu-id="a81b1-115">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="a81b1-116">向团队中添加新成员。</span><span class="sxs-lookup"><span data-stu-id="a81b1-116">Add a new member to the team.</span></span>|
|[<span data-ttu-id="a81b1-117">获取团队成员</span><span class="sxs-lookup"><span data-stu-id="a81b1-117">Get team member</span></span>](../api/team-get-members.md) | <span data-ttu-id="a81b1-118">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a81b1-118">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="a81b1-119">获取团队中的成员。</span><span class="sxs-lookup"><span data-stu-id="a81b1-119">Get a member in the team.</span></span>|
|[<span data-ttu-id="a81b1-120">更新成员角色</span><span class="sxs-lookup"><span data-stu-id="a81b1-120">Update team member's role</span></span>](../api/team-update-members.md)|[<span data-ttu-id="a81b1-121">conversationMember</span><span class="sxs-lookup"><span data-stu-id="a81b1-121">conversationMember</span></span>](../resources/conversationmember.md)|<span data-ttu-id="a81b1-122">将成员更改为所有者或返回为常规成员。</span><span class="sxs-lookup"><span data-stu-id="a81b1-122">Change a member to an owner or back to a regular member.</span></span>|
|[<span data-ttu-id="a81b1-123">删除团队成员</span><span class="sxs-lookup"><span data-stu-id="a81b1-123">Remove team member</span></span>](../api/team-delete-members.md)|<span data-ttu-id="a81b1-124">无</span><span class="sxs-lookup"><span data-stu-id="a81b1-124">None</span></span>|<span data-ttu-id="a81b1-125">删除团队中的一个现有成员。</span><span class="sxs-lookup"><span data-stu-id="a81b1-125">Remove an existing member from the team.</span></span>|
|[<span data-ttu-id="a81b1-126">列出频道成员</span><span class="sxs-lookup"><span data-stu-id="a81b1-126">List channel members</span></span>](../api/channel-list-members.md) | <span data-ttu-id="a81b1-127">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a81b1-127">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="a81b1-128">获取频道中的所有成员列表。</span><span class="sxs-lookup"><span data-stu-id="a81b1-128">Get the list of all members in a channel.</span></span>|
|[<span data-ttu-id="a81b1-129">添加频道成员</span><span class="sxs-lookup"><span data-stu-id="a81b1-129">Add channel member</span></span>](../api/channel-post-members.md) | [<span data-ttu-id="a81b1-130">conversationMember</span><span class="sxs-lookup"><span data-stu-id="a81b1-130">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="a81b1-131">向频道添加成员。</span><span class="sxs-lookup"><span data-stu-id="a81b1-131">Add a member to a channel.</span></span> <span data-ttu-id="a81b1-132">仅支持 membershipType 为 `private` 的 `channel`。</span><span class="sxs-lookup"><span data-stu-id="a81b1-132">Only supported for `channel`with membershipType of `private`.</span></span>|
|[<span data-ttu-id="a81b1-133">获取频道成员</span><span class="sxs-lookup"><span data-stu-id="a81b1-133">Get channel member</span></span>](../api/channel-get-members.md) | <span data-ttu-id="a81b1-134">[conversationMember](conversationmember.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a81b1-134">[conversationMember](conversationmember.md) collection</span></span> | <span data-ttu-id="a81b1-135">获取频道中的成员。</span><span class="sxs-lookup"><span data-stu-id="a81b1-135">Get a member in a channel.</span></span>|
|[<span data-ttu-id="a81b1-136">更新频道成员角色</span><span class="sxs-lookup"><span data-stu-id="a81b1-136">Update channel member's role</span></span>](../api/channel-update-members.md) | [<span data-ttu-id="a81b1-137">conversationMember</span><span class="sxs-lookup"><span data-stu-id="a81b1-137">conversationMember</span></span>](conversationmember.md) | <span data-ttu-id="a81b1-138">更新频道成员的属性。</span><span class="sxs-lookup"><span data-stu-id="a81b1-138">Update the properties of a member of the channel.</span></span> <span data-ttu-id="a81b1-139">仅支持 membershipType 为 `private` 的频道。</span><span class="sxs-lookup"><span data-stu-id="a81b1-139">Only supported for channel with membershipType of `private`.</span></span>|
|[<span data-ttu-id="a81b1-140">删除频道成员</span><span class="sxs-lookup"><span data-stu-id="a81b1-140">Remove channel member</span></span>](../api/channel-delete-members.md) | <span data-ttu-id="a81b1-141">无</span><span class="sxs-lookup"><span data-stu-id="a81b1-141">None</span></span> | <span data-ttu-id="a81b1-142">从频道中删除一个成员。</span><span class="sxs-lookup"><span data-stu-id="a81b1-142">Delete a member from a channel.</span></span> <span data-ttu-id="a81b1-143">仅支持用于 `private` 的 `channelType`。</span><span class="sxs-lookup"><span data-stu-id="a81b1-143">Only supported for `channelType` of `private`.</span></span>|

## <a name="properties"></a><span data-ttu-id="a81b1-144">属性</span><span class="sxs-lookup"><span data-stu-id="a81b1-144">Properties</span></span>

| <span data-ttu-id="a81b1-145">属性</span><span class="sxs-lookup"><span data-stu-id="a81b1-145">Property</span></span>   | <span data-ttu-id="a81b1-146">类型</span><span class="sxs-lookup"><span data-stu-id="a81b1-146">Type</span></span> |<span data-ttu-id="a81b1-147">说明</span><span class="sxs-lookup"><span data-stu-id="a81b1-147">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a81b1-148">id</span><span class="sxs-lookup"><span data-stu-id="a81b1-148">id</span></span>|<span data-ttu-id="a81b1-149">String</span><span class="sxs-lookup"><span data-stu-id="a81b1-149">String</span></span>| <span data-ttu-id="a81b1-150">只读。</span><span class="sxs-lookup"><span data-stu-id="a81b1-150">Read-only.</span></span> <span data-ttu-id="a81b1-151">用户的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="a81b1-151">Unique ID of the user.</span></span>|
|<span data-ttu-id="a81b1-152">displayName</span><span class="sxs-lookup"><span data-stu-id="a81b1-152">displayName</span></span>| <span data-ttu-id="a81b1-153">string</span><span class="sxs-lookup"><span data-stu-id="a81b1-153">string</span></span> | <span data-ttu-id="a81b1-154">用户的显示名称。</span><span class="sxs-lookup"><span data-stu-id="a81b1-154">The display name of the user.</span></span> |
|<span data-ttu-id="a81b1-155">角色</span><span class="sxs-lookup"><span data-stu-id="a81b1-155">roles</span></span>| <span data-ttu-id="a81b1-156">string 集合</span><span class="sxs-lookup"><span data-stu-id="a81b1-156">string collection</span></span> | <span data-ttu-id="a81b1-157">该用户的角色。</span><span class="sxs-lookup"><span data-stu-id="a81b1-157">The roles for that user.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a81b1-158">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a81b1-158">JSON representation</span></span>

<span data-ttu-id="a81b1-159">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a81b1-159">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.conversationMember",
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

